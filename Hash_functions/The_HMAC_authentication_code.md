
copy message, key (without quotes - ") from the server response
echo -n "message" | openssl dgst -sha512 -hmac "key"