FROM php:7.2-apache

RUN chmod a+x /opt/entrypoints.sh
RUN /bin/bash -c "source /opt/entrypoints.sh /etc/apache2/ssl_keys localhost"
RUN a2enmod ssl
RUN a2ensite ssl

CMD["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
