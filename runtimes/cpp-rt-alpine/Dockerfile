# C++ Runtime Image for Alpine Linux 3.8
#
# This Docker image contains the standard C/C++ runtime libraries, including
# support for C++11 libraries.
#
FROM alpine:3.8
LABEL maintainer "Braden Hitchcock <developer.hitchcock@gmail.com>"

RUN apk add --update \
        libstdc++ \
        libc++ \
    && rm -rf /var/apk/cache/*

