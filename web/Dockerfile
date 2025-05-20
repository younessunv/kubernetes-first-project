FROM php:8.2-apache

RUN docker-php-ext-install mysqli pdo pdo_mysql

RUN a2enmod rewrite

RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf

RUN service apache2 restart

COPY index.php /var/www/html/

RUN chmod -R 755 /var/www/html && chown -R www-data:www-data /var/www/html
