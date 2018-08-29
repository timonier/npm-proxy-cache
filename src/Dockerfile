FROM timonier/node:latest

LABEL \
    maintainer="Morgan Auchede <morgan.auchede@gmail.com>"

RUN set -e -u -x \
\
    # Install npm-proxy-cache
\
    && yarn global add npm-proxy-cache \
\
    # Clean
\
    && rm -f -r /tmp/* "$(yarn cache dir)"/*
