# Inpsired from https://github.com/schickling/dockerfiles/blob/master/mailcatcher/Dockerfile
FROM ruby:alpine

LABEL maintainer="Pierre-Louis Launay <laupi.frpar@gmail.com>"

ARG VERSION=0.6.5
RUN set -xe \
    && apk add --no-cache \
        libstdc++ \
        sqlite-libs \
    && apk add --no-cache --virtual .build-deps \
        build-base \
        sqlite-dev \
    && gem install mailcatcher -v ${VERSION} \
    && apk del .build-deps

CMD ["mailcatcher", "--no-quit", "--foreground", "--ip=0.0.0.0"]

EXPOSE 1025 1080
