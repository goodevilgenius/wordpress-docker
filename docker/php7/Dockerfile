FROM php:7.1.4-apache
RUN docker-php-ext-install mysqli \
    && a2enmod rewrite \
    && curl -o /usr/local/bin/wp https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar \
    && chmod +x /usr/local/bin/wp \
    && apt-get update \
    && apt-get install -y less
