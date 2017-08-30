FROM nginx:alpine

RUN rm /etc/nginx/conf.d/*

COPY proxy.conf /etc/nginx/conf.d/

COPY selfsigned.crt  /etc/nginx/
COPY selfsigned.key  /etc/nginx/
COPY dhparam.pem  /etc/nginx/