# PBKDF2 with non standard number of iterations

1. `nc <ip> port`
2. `echo <message> > data.enc`
3. `openssl enc -d -a -aes-256-cbc -in data.enc -k <password> -pbkdf2 -iter <iterations>`