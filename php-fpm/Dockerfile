# php-fpm
FROM php:7.3-fpm

LABEL maintainer="ElHaouari Mohammed <mohammed.elhaouari@dzconseil.com>"

# Install the PHP pdo_mysql extention
RUN docker-php-ext-install pdo_mysql \
    # Install the PHP pdo_mysql extention
    && docker-php-ext-install bcmath
# Install the PHP pdo_pgsql extention
# && docker-php-ext-install pdo_pgsql \
# Install the PHP pdo_sqlite extention
# && docker-php-ext-install pdo_sqlite \
# Install the PHP mbstring extention
# && docker-php-ext-install mbstring \
# Install the PHP mbstring extention
# && docker-php-ext-install curl \
# Enable Exif PHP extentions requirements
# && docker-php-ext-install exif
# Install the PHP gd library
# && docker-php-ext-configure gd \
# --with-jpeg-dir=/usr/lib \
# --with-freetype-dir=/usr/include/freetype2 && \
# docker-php-ext-install gd


#
#--------------------------------------------------------------------------
# Final Touch
#--------------------------------------------------------------------------
#
COPY ./custom.ini /usr/local/etc/php/conf.d

WORKDIR /var/www

CMD ["php-fpm"]

EXPOSE 9000