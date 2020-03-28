# FROM php:latest
FROM php:7-fpm
RUN apt-get update && apt-get install -y \
    vim \
    unzip \
    iputils-ping \
    git
RUN docker-php-ext-install pdo_mysql
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
