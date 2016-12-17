FROM node:7.2-alpine

MAINTAINER Milos Zivanovic <miloszivanovic@gmail.com>

RUN apk update
RUN apk add git curl

WORKDIR /opt/app

RUN npm install --global yarn

RUN npm install -g gulp

WORKDIR /tmp/app/

VOLUME ["/tmp/app/"]
