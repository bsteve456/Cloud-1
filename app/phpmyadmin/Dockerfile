FROM phpmyadmin:fpm
COPY ./config.inc.php /var/www/html
RUN rm /var/www/html/config.sample.inc.php
VOLUME /usr/share/phpmyadmin
RUN cp -r /var/www/html/* /usr/share/phpmyadmin
