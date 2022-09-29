ARG ARCH=
FROM ${ARCH}node:16-alpine

RUN apk add --update file libunwind build-base curl py-pip tzdata zeromq-dev git openssh-client \
    && rm -rf /var/cache/apk/* \
    && cp /usr/share/zoneinfo/Europe/Berlin /etc/localtime \
    && echo "Europe/Berlin" >  /etc/timezone


CMD [ "top", "-b"]
