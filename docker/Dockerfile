FROM php:8.2-fpm

RUN apt-get update \
    && apt-get install -y git unzip libzip-dev \
    && docker-php-ext-install zip pdo_mysql

RUN pecl install redis && docker-php-ext-enable redis

RUN pecl install xdebug && docker-php-ext-enable xdebug

