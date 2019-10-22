FROM php:7.2-fpm-stretch

COPY ./php7.2/php.ini /usr/local/etc/php/

RUN mkdir -p /var/log/php_log

RUN apt-get update \
    && apt-get install -y --no-install-recommends \

    # redis
    && pecl install -o -f redis-4.3.0 \
    && docker-php-ext-enable redis

# Clear cache
RUN apt-get clean && rm -rf /var/lib/apt/lists/*