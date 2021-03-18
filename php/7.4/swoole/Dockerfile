FROM axerl/php-cli:7.4

RUN set -ex \
    && apt-get update \
    && apt-get install -y php7.4-dev php-pear \
    && pecl install swoole \
    && echo "memory_limit=1G" > /etc/php/7.4/cli/conf.d/00-default.ini \
    && echo "extension=swoole.so" > /etc/php/7.4/cli/conf.d/50-swoole.ini \
    && apt-get clean \
    && php -v \
    && php -m \
    && php --ri swoole