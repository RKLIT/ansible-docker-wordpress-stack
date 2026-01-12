#Image Apache with PHP
FROM php:8.2-apache

#Install additional extensions for PHP
RUN docker-php-ext-install mysqli pdo pdo_mysql

#Enable mod_rewrite
RUN a2enmod rewrite

#Copy the default directory to DocumentRoot Apache
COPY ./app /var/www/html/

#Rules
RUN chown -R www-data:www-data /var/www/html

#Default Port - 80
EXPOSE 80  
