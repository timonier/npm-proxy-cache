FROM alpine:3.4

LABEL \
    maintainer="Morgan Auchede <morgan.auchede@gmail.com>"

ENV \
    NPM_PROXY_CACHE_VERSION=0.4.2

RUN set -x \

    # Install packages

    && apk add --no-cache --no-progress --virtual build_deps \
           curl \

    && apk add --no-cache --no-progress \
           ca-certificates \
           nodejs \

    # Install npm-proxy-cache

    && npm install -g \
           npm-proxy-cache@${NPM_PROXY_CACHE_VERSION} \

    # Install timonier/dumb-entrypoint

    && curl -sL "https://github.com/timonier/dumb-entrypoint/raw/master/bin/installer" | INSTALL_DIRECTORY="/usr/sbin" sh -s install \

    # Clean

    && apk del --no-progress \
          build_deps

ENTRYPOINT [ "dumb-init" , "--" , "dumb-entrypoint" , "npm-proxy-cache" ]
