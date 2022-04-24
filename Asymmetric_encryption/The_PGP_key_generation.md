# The PGP key generation

1. `nc <ip> <port>` copy string
2. `gpg --gen-key` put string in name, put random garbage in email
3. `gpg --export --armor <string>` copy to clipboard
4. paste into `nc <ip> <port>`