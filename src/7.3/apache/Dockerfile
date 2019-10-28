FROM jrobinsonc/php:7.3-apache

RUN apt-get update; \
    docker-php-ext-install bcmath; \
    rm -rf /var/lib/apt/lists/*;
