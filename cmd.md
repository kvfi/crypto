### Générer un certificat auto-signé

`openssl x509 -req -in mondomaine.csr -out mondomaine.pem -CA ca.crt -CAkey mykey.pem -CAcreateserial -CAserial ca.srl -days 90`
