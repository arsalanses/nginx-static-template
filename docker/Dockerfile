FROM nginx:1.25.3-alpine-slim

COPY ./docker/default.conf /etc/nginx/conf.d/default.conf
COPY ./docker/nginx.conf /etc/nginx/nginx.conf
COPY ./docker/.htpasswd /etc/nginx/.htpasswd

COPY . /usr/share/nginx/html

# docker build -t "landing:latest" -f docker/Dockerfile .
# docker run --rm -d --network web -p8080:80 --name landing landing:latest
