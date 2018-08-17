# Dockerfile
FROM alpine:3.8
LABEL maintainer "developer.hitchcock@gmail.com"

# Setup Environment
ENV HOME /root

# Install all build dependencies
RUN apk add --update \
        build-base \
        maven \
    && rm -rf /var/cache/apk/*

WORKDIR /src
