# docker-nginx-ssl

## To generate self signed certificate run following command as root

```bash
openssl req -batch -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/nginx.key -out /etc/ssl/certs/nginx.crt 
```

### If you already have ssl cert and key files update line no. 15 and 16 in docker-compose file

### To start the server run following command

```bash
docker-compose up -d --build --force-recreate
```
