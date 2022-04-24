# Encryption with the PGP key
## this one is a bit fucked
1. `nc <ip> <port>` copy string into data.txt, copy key into pub.pem
2. `gpg --import pub.pem`
3. `gpg --encrypt --armor --recipient contact@cyberskiller.com data.txt` mail is important here, try piping instead of reading data from file