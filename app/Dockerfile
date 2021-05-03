FROM php:7.4.15-fpm-alpine3.13

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /app

COPY . /app

RUN composer install --no-dev --optimize-autoloader

