FROM httpd:latest

MAINTAINER SaravAK (aksarav@middlewareinventory.com)

COPY httpd.conf /usr/local/apache2/conf/httpd.conf
COPY vhost80.conf /usr/local/apache2/conf/vhost80.conf
COPY base_vhost.conf /usr/local/apache2/conf/base_vhost.conf

RUN mkdir -p /usr/local/apache2/conf/sites/

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]