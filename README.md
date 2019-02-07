# Docker PHP-FPM 7.1 & Nginx 1.12 on Alpine Linux 3.7

Build on [Alpine Linux](http://www.alpinelinux.org/).

Usage
-----
Start the Docker containers:

Run :

```
docker run -p 80:80 ramadhan/docker-php7.1-nginx-alpine:latest
```

Docker Compose:

```
version: "2"
services: 
  web:
    image: "ramadhan/docker-php7.1-nginx-alpine:latest"
    container_name: web-rama
    ports:
        - "80:80"
        - "443:443"
```