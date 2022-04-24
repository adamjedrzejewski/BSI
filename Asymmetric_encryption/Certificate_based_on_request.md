# Certificate based on request

1. `nc <ip> <port>` copy request into client.csr
2. `openssl genrsa -out ca.key 2048`
3. `openssl req -new -x509 -key ca.key -out ca.crt`
4. `openssl x509 -req -CAkey ca.key -CA ca.crt -in client.csr -CAcreateserial -out client.crt`
5. copy client.csr into `nc <ip> <port>`