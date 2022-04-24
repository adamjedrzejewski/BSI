# Certificate with a given Common Name field

1. `nc <ip> <port>` copy the string
2. `openssl genrsa -out ca.key 2048`
3. `openssl req -new -x509 -key ca.key -out ca.crt` put string in field "Common Name"
4. copy ca.crt
5. paste into `nc <ip> <port>`