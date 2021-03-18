ARG UBUNTU_VERSION

FROM ubuntu:${UBUNTU_VERSION}

RUN apt-get update \
    && ln -fs /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && apt-get install -y curl \
        wget \
        php7.4 \
        php7.4-cli \
        php7.4-curl \
        php7.4-json \
        php7.4-mbstring \
        php7.4-opcache \
        php7.4-xml \
        php7.4-zip \
        php7.4-bcmath \
        php7.4-mysql \
        php7.4-dom \
        php7.4-gd \
        php7.4-redis \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*