# Data decryption with the 3DES algorithm

1. `nc <ip> port`
2. `echo <message> > data.enc`
3. `openssl enc -d -a -in data.enc -k <password> -pbkdf2 -des-ede3-ecb`