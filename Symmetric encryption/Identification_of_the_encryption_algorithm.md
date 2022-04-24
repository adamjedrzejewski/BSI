# Identification of the encryption algorithm

1. `nc <ip> port` **DON'T CLOSE THE CONNECTION**
2. `echo <message> > data.enc`
3. `echo <password> > pwd.pass`
4. `bash script.sh`
5. find cipher that didn't fail, copy it
6. paste it into `nc <ip> port`


```
ciphers=(
-aes-128-ecb
-aes-192-ecb
-aes-256-ecb
-aria-128-ecb
-aria-192-ecb
-aria-256-ecb
-bf-ecb
-camellia-128-ecb
-camellia-192-ecb
-camellia-256-ecb
-cast5-ecb
-des-ecb
-des-ede-ecb
-des-ede3-ecb
-rc2-ecb
-seed-ecb
-sm4-ecb
)
for cipher in ${ciphers[@]}
do
        echo "---"
        echo $cipher
        openssl enc -d -a $cipher -in data.enc -kfile pwd.pass -pbkdf2
        echo ""
done;
```