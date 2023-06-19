FROM nginx:latest

RUN mkdir -p /var/www/html && rm -rfvd /etc/nginx/conf.d/default.conf

COPY src /var/www/html

COPY docker/nginx/conf.d/default.conf /etc/nginx/conf.d/default.conf

