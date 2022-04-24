# Decryption using PBKDF1 algorithm

1. `nc <ip> port`
2. `echo <message> > data.enc`
3. `openssl enc -d -aes-256-ecb -k <password> -in data.enc -a -iter <iterations>`