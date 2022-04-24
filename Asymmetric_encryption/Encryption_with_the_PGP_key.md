# Encryption with the PGP key
## broken
1. `nc <ip> <port>` copy string into data.txt, copy key into pub.pem
2. `gpg --import pub.pem`
3. `gpg --encrypt --armor --recipient cyberskiller data.txt` (new line?)