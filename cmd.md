### EJBCA (Docker)
`docker run -it -p 9812:8080 -p 443:8443 -h localhost -e TLS_SETUP_ENABLED="simple" primekey/ejbca-ce`

### Générer un certificat auto-signé

`openssl x509 -req -in mondomaine.csr -out mondomaine.pem -CA ca.crt -CAkey mykey.pem -CAcreateserial -CAserial ca.srl -days 90`
