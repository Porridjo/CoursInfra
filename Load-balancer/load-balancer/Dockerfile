FROM debian:latest

RUN apt-get update && apt-get install apache2 -y

RUN a2enmod proxy
RUN a2enmod proxy_http
RUN a2enmod proxy_balancer
RUN a2enmod lbmethod_byrequests

COPY nodejs_ipshow.conf /etc/apache2/sites-available/000-default.conf

EXPOSE 80

CMD apachectl -D FOREGROUND