# alpine-nginx

[![Docker Stars](https://img.shields.io/docker/stars/jonnybgod/alpine-nginx.svg)]()
[![Docker Pulls](https://img.shields.io/docker/pulls/jonnybgod/alpine-nginx.svg)]()

Docker container with nginx pre-installed feat: ssl, http2, gzip

## Usage

```dockerfile
FROM jonnybgod/alpine-nginx:latest

WORKDIR /src

ADD . .
RUN cp nginx.conf /etc/nginx/nginx.conf

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
```
