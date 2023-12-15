![nginx 1.16](https://img.shields.io/badge/nginx-1.16-brightgreen.svg)
![php 7.3](https://img.shields.io/badge/php-7.3-brightgreen.svg)
![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)

# Docker PHP-FPM 7 & Nginx on Alpine Linux
Example PHP-FPM 7 & Nginx container image for Docker, built on [Alpine Linux](https://www.alpinelinux.org/).

Repository: https://github.com/cvtung/docker-php7-fpm-nginx-alpine

## Goal of this project
The goal of this container image is to provide an example for running Nginx and PHP-FPM in a container which follows
the best practices and is easy to understand and modify to your needs.

## Usage

Start the Docker container:

    docker run -p 80:8080 tungcv/php7-fpm-nginx-alpine

See the PHP info on http://localhost, or the static html page on http://localhost/test.html

Or mount your own code to be served by PHP-FPM & Nginx

    docker run -p 80:8080 -v ~/my-codebase:/var/www/html tungcv/php7-fpm-nginx-alpine