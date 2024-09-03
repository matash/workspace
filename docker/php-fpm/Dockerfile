FROM php:8.2-fpm

RUN apt-get update && apt-get install -y libpq-dev unzip
RUN docker-php-ext-install pdo pdo_mysql

# Install composer
COPY --from=composer /usr/bin/composer /usr/bin/composer

WORKDIR /var/www