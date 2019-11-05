FROM php:7.3-apache
RUN docker-php-ext-install mysqli pdo pdo_mysql
ADD php.ini /usr/local/etc/php/php.ini
ADD https://github.com/mailhog/mhsendmail/releases/download/v0.2.0/mhsendmail_linux_amd64 /usr/local/bin/mhsendmail
RUN chmod +x /usr/local/bin/mhsendmail

RUN apt-get update && apt-get install -y libmagickwand-dev --no-install-recommends