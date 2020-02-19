# Docker Laravel Image

[![Build Status](https://travis-ci.org/jrobinsonc/docker-laravel-image.svg?branch=master)](https://travis-ci.org/jrobinsonc/docker-laravel-image)

<https://hub.docker.com/r/jrobinsonc/laravel>

## Includes

* PHP extensions required by Laravel.
* Composer
* Node v12
* NPM v6

**Image Variants**

* PHP 7.3 with Apache → `jrobinsonc/laravel:7.3-apache`

## How to use

**Start the container:**

```shell
docker run \
  -p 80:80 \
  -p 443:443 \
  -v $(pwd):/var/www/html \
  jrobinsonc/laravel:7.3-apache
```