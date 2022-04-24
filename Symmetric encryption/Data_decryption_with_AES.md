# Data decryption with AES

1. `nc <ip> <port>`
2. `echo <message> > data.enc`
3. `openssl enc -aes-256-ecb -d -a -in data.enc -K <key>`