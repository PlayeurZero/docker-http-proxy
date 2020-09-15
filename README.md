# http to https proxy for Docker apps

A `docker-compose.yml` and a nginx configuration to proxy-pass a Docker HTTP application to HTTPS.

## Run

Put your certificate in `web/certificates/web.crt`.  
Put your key in `web/certificates/web.key`.

Run&#x202f;:

```sh
docker-compose up
```

**Note**

To generate your own certificate, use this command&#x202f;:

```sh
sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./web/certificates/web.key -out ./web/certificates/web.crt
```
