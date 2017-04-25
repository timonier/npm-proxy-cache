FROM node:alpine

LABEL \
    maintainer="Morgan Auchede <morgan.auchede@gmail.com>"

ENV \
    NPM_PROXY_CACHE_VERSION=latest

RUN set -eux \

    # Install packages

    && apk add --no-cache --no-progress --virtual BUILD_DEPS \
           curl \

    && apk add --no-cache --no-progress \
           ca-certificates \

    # Install dumb-entrypoint

    && curl --location "https://github.com/timonier/dumb-entrypoint/raw/master/bin/installer" | INSTALL_DIRECTORY="/usr/sbin" sh -s install \

    # Install npm-proxy-cache

    && export $(curl "https://raw.githubusercontent.com/timonier/version-lister/release/generated/npm-proxy-cache/${NPM_PROXY_CACHE_VERSION}" | xargs) \

    && npm install -g \
           "npm-proxy-cache@${NPM_PROXY_CACHE_VERSION}" \

    # Clean

    && apk del --no-progress \
          BUILD_DEPS

ENTRYPOINT [ "dumb-init" , "--" , "dumb-entrypoint" ]
