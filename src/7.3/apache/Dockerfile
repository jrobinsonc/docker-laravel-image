FROM jrobinsonc/php:7.3-apache

RUN apt-get update; \
    curl -sL https://deb.nodesource.com/setup_12.x | bash -; \
    apt-get install -y nodejs mariadb-client; \
    docker-php-ext-install bcmath pdo_mysql; \
    rm -rf /var/lib/apt/lists/*;
