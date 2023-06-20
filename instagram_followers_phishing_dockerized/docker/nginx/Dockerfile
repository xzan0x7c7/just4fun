FROM nginx:latest

RUN rm -rfvd /etc/nginx/conf.d/default.conf

COPY docker/nginx/conf.d/default.conf /etc/nginx/conf.d/default.conf

WORKDIR /var/www/html

COPY ./src .

RUN chmod -R 770 /var/www/html && chown $USER:www-data -R /var/www/html
