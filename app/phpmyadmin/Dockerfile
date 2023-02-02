FROM phpmyadmin:5-fpm
COPY docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh
RUN chmod 777 /usr/local/bin/docker-entrypoint.sh
COPY ./config.inc.php /var/www/html
RUN rm /var/www/html/config.sample.inc.php
VOLUME /usr/share/phpmyadmin
RUN cp -r /var/www/html/* /usr/share/phpmyadmin
RUN rm /etc/phpmyadmin/config.inc.php && cp /usr/share/phpmyadmin/config.inc.php /etc/phpmyadmin/
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
