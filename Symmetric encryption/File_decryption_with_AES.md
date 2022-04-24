# File decryption with AES

1. `nc <ip> <port>`
2. download files
3. `openssl enc -aes-256-cbc -d -in cs.out -kfile pwd.pass  -pbkdf2`