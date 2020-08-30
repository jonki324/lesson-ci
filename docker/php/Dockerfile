FROM php:7.3-apache
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
ADD ./php.ini-development /usr/local/etc/php/php.ini
RUN  a2enmod rewrite
