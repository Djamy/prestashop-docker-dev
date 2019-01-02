FROM prestashop/prestashop:1.6.1.23
LABEL maintainer="Djamy <yo@dja.my>"

RUN pecl install xdebug-2.5.5 \
    && docker-php-ext-enable xdebug
    
RUN echo "xdebug.remote_enable=true" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini \
    && echo "xdebug.remote_port=5902" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini \
    && echo "xdebug.remote_host=docker.host" >> /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
