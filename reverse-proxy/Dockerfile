FROM jslucas/apache_shib_base

RUN yum -y update; yum clean all
RUN yum -y install sudo net-tools

EXPOSE 80

# httpd configs
COPY base_vhost.conf /etc/httpd/conf.d/ 

COPY  httpd.conf /usr/local/httpd/conf/

# start services
CMD ["httpd", "-D", "FOREGROUND"]
