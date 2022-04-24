# Key generation on elliptic curves

1. `openssl ecparam -name prime256v1 -genkey -out priv.pem`
2. `openssl ec -in priv.pem -out pub.pem -pubout`
3. `cat pub.pem > solution`
4. `echo >> solution`
5. `cat priv.pem >> solution`
6. copy paste solution into `nc <ip> <port>`