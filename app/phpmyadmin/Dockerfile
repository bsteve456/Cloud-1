FROM phpmyadmin:5-fpm
RUN rm /etc/phpmyadmin/config.inc.php
COPY ./config.inc.php /etc/phpmyadmin/config.inc.php
RUN chmod 777 /var/www/html/tmp
