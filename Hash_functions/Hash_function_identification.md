
`nc <ip> <port>`
copy `string`, `result` (without quotes - ") from the server response
import hashlib

word = '`string`'.encode('utf-8')
key = '`result`'

for alg in hashlib.algorithms_available:
    try:
        hash_instance = hashlib.new(alg)
        hash_instance.update(word)
        if hash_instance.hexdigest() == key:
            print(f'Alg: {alg}')
    except:
        print(f"Execption: {alg}")
