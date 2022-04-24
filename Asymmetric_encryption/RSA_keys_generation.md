# RSA keys generation

1. `openssl genrsa -out priv.pem 4096`
2. `openssl rsa -in priv.pem -pubout -out pub.pem`
3. `cat pub.pem > solution`
4. `echo >> solution`
5. `cat priv.pem >> solution`
6. copy paste solution into `nc <ip> <port>`