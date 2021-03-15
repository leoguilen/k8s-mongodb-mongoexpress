## TLS certificate
Generate TLS certificate secret for kubernetes ingress:

```sh
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
    -out <CERTIFICATE_NAME>.crt \
    -keyout <CERTIFICATE_NAME>.key \
    -subj "/CN=<DNS_NAME>/O=<CERTIFICATE_NAME>"
```