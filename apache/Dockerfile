# Imagen base: Debian + Apache + PHP
FROM php:8.2-apache

# Extensiones de PHP que necesita la aplicación
RUN docker-php-ext-install pdo_mysql

# Solo lo que se publica: nunca .git, README ni el .sql
COPY css/ /var/www/html/css/
COPY img/ /var/www/html/img/
COPY *.html *.php /var/www/html/
