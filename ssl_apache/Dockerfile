FROM php:7.2-apache

COPY ./src /var/www/html
COPY ./conf/ssl.conf /etc/apache2/sites-available/ssl.conf
COPY ./conf/entrypoint.sh /opt/entrypoint.sh

RUN chmod a+x /opt/entrypoint.sh
RUN /bin/bash -c "source /opt/entrypoint.sh /etc/apache2/ssl_keys 172.21.39.250"
RUN a2enmod ssl
RUN a2enmod rewrite
RUN a2ensite ssl
RUN /bin/bash -c "/usr/sbin/apache2ctl -D FOREGROUND"
