
copy string (without quotes - ") from the server response

import hashlib
h = hashlib.sha3_512()
h.update("string".encode("utf-8"))
h.digest()
h.hexdigest()

echo -n "string" | openssl dgst -sha3-512