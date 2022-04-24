# Encryption with the public key

1. `nc <ip> <port>` save public key in pub.pem, save string in data.txt
2. `openssl rsautl -encrypt -in data.txt -inkey pub.pem -pubin -out data.enc -oaep`
3. `base64 -w0 data.enc` copy to clipboard
4. paste into `nc <ip> <port>`