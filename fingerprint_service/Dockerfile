FROM dahirmuhammaddahir/secureng-php-apache

WORKDIR /var/www/html

COPY . .

RUN composer update
RUN composer install

RUN cd thirdparty/grpc-fingerprint-engine/src/php/
RUN composer update
RUN composer install

RUN apt update
RUN apt install -y net-tools

