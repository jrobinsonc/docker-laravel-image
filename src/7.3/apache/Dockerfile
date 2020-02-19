# Based on
# https://laravel.com/docs/6.x/installation#server-requirements
FROM jrobinsonc/php:7.3-apache

RUN set -ex; \
    apt-get update; \
    curl -sL https://deb.nodesource.com/setup_12.x | bash -; \
    apt-get install -y --no-install-recommends \
      nodejs \
      mariadb-client \
    ; \
    rm -rf /var/lib/apt/lists/*;

RUN set -eux; \
    docker-php-ext-install -j "$(nproc)" \
      bcmath \
      pdo_mysql \
    ;

RUN a2enmod rewrite expires headers
