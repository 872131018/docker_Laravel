FROM ubuntu:latest

RUN apt-get update && apt-get install -y software-properties-common && \
    add-apt-repository -y ppa:ondrej/php && \
    apt-get update && \
    apt-get install -y --allow-unauthenticated \
    php7.1 php7.1-fpm php7.1-mysql mcrypt curl php7.1-curl php7.1-mbstring

RUN sed -i -e 's/listen = \/run\/php\/php7.0-fpm.sock/listen = 0.0.0.0:9000/g' /etc/php/7.0/fpm/pool.d/www.conf \
    && sed -i -e 's/;daemonize = yes/daemonize = no/g' /etc/php/7.0/fpm/php-fpm.conf

EXPOSE 9000
