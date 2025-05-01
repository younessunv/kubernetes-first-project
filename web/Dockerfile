# Use the official PHP image with Apache
FROM php:8.2-apache

# Install mysqli and pdo_mysql extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Enable Apache modules (optional)
RUN a2enmod rewrite

# Set the ServerName directive to suppress Apache warnings
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf

# Restart Apache to apply changes
RUN service apache2 restart
