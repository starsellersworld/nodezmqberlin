FROM node:14-alpine

RUN apk add --update file libunwind build-base python tzdata zeromq-dev \
    && rm -rf /var/cache/apk/* \
    && cp /usr/share/zoneinfo/Europe/Berlin /etc/localtime \
    && echo "Europe/Berlin" >  /etc/timezone


CMD [ "top", "-b"]
