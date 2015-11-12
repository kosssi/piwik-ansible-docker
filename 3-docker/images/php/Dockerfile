FROM php:5.6-fpm

MAINTAINER Simon Constans "simon@constans.io"

RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng12-dev && \
    docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ --with-png-dir=/usr/include/ && \
    docker-php-ext-install pdo pdo_mysql mbstring gd && \
    echo "always_populate_raw_post_data=-1" >> /usr/local/etc/php/php.ini
