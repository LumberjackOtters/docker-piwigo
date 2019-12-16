# FROM php:7-fpm-alpine
FROM php:5-fpm-alpine
RUN apk add libpng-dev freetype-dev libjpeg-turbo-dev \
    && docker-php-ext-install mysqli \
    && docker-php-ext-enable mysqli \
    && docker-php-ext-configure gd --with-gd --with-webp-dir --with-jpeg-dir \
    --with-png-dir --with-freetype-dir \
    --enable-gd-native-ttf \
    && docker-php-ext-install gd \
    && docker-php-ext-enable gd \
    && docker-php-ext-install exif \
    && docker-php-ext-enable exif