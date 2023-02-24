FROM mcr.microsoft.com/devcontainers/base:bullseye

ARG HUGO_VERSION=0.110.0

RUN wget -O /tmp/hugo.tar.gz https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_extended_${HUGO_VERSION}_Linux-64bit.tar.gz
RUN tar xf /tmp/hugo.tar.gz --directory /usr/local/bin

EXPOSE 1313
