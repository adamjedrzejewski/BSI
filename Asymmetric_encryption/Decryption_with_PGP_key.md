# Decryption with PGP key

1. `gpg --gen-key`
2. `gpg --export --armor <name>`
3. `nc <ip> <port>` paste public key, save to data.enc
4. `gpg --decrypt data.enc`