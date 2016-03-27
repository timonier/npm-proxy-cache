FROM alpine:3.3
MAINTAINER Morgan Auchede <morgan.auchede@gmail.com>

ENV \
    NPM_PROXY_CACHE_VERSION=0.4.2

RUN set -x \

    # Prepare system

    && apk add -U \

    # Install packages

    && apk add \
           nodejs \

    # Install npm-proxy-cache

    && npm install -g \
           npm-proxy-cache@$NPM_PROXY_CACHE_VERSION \

    # Clean

    && rm -rf \
           /var/cache/apk/*

COPY ./rootfs /

ENTRYPOINT [ "/entrypoint.sh" ]
