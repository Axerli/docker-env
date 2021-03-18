FROM axerl/php-cli:7.4

RUN apt-get update \
    && apt-get -y --no-install-recommends install php7.4-fpm \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

COPY www.conf /etc/php/7.4/fpm/pool.d/www.conf

CMD ["/usr/sbin/php-fpm7.4", "-O" ]

EXPOSE 9000