FROM alpine:3.3
MAINTAINER Morgan Auchede <morgan.auchede@gmail.com>

ENV \
    NPM_PROXY_CACHE_VERSION=0.4.2

RUN set -x \

    # Install packages

    && apk add --no-cache --no-progress \
           nodejs \

    # Install npm-proxy-cache

    && npm install -g \
           npm-proxy-cache@$NPM_PROXY_CACHE_VERSION

COPY ./rootfs /

ENTRYPOINT [ "/entrypoint.sh" ]
