# Encrypted Zip file

1. download the file 
2. `zip2john <file> > john.pass`
3. `wget https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt`
4. `john --wordlist=rockyou.txt john.pass` it will give you a password
5. `unzip <file>` will ask for password
6. `cat secret.txt`