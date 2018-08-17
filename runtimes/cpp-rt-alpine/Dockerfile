# C++ Runtime Image for Alpine Linux 3.8
#
# This Docker image contains the standard C/C++ runtime libraries, including
# support for C++11 libraries.
#
FROM alpine:3.8
LABEL maintainer "Braden Hitchcock <developer.hitchcock@gmail.com>"

RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories \
    && apk update \
    && apk add --no-cache --update \
        libstdc++ \
        libc++ \
    && rm -rf /var/apk/cache/*

