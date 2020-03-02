FROM php:7.2-fpm

RUN apt-get update
RUN apt-get install vim -y
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install pdo_mysql
RUN pecl install yaf
RUN pecl install swoole

ADD php.ini /usr/local/etc/php/

WORKDIR /home/site/