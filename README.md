# crypt
Encrypt/decrypt whatever online without SMS and registration

#### OpenSSL encrypt/decrypt

Encrypt:
```shell script
echo -n "$@" | # input text
 openssl enc \
  -e `# encode` \
  -aes-256-cbc `# ciphername` \
  -base64 `# base64` \
  -salt # use salt (randomly generated or provide with -S option) when encrypting (this is the default).
```
