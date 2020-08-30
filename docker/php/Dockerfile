FROM php:7.3-apache
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
RUN  a2enmod rewrite
RUN apt-get update && apt-get install -y zip unzip git libicu-dev && docker-php-ext-install intl
ADD ./php.ini-development /usr/local/etc/php/php.ini
