FROM node:7.2

MAINTAINER Milos Zivanovic <miloszivanovic@gmail.com>

RUN apt-get update
RUN apt-get install -y git build-essential curl

WORKDIR /opt/app

RUN curl -o- -L https://yarnpkg.com/install.sh | bash

RUN npm install -g gulp --save-dev

WORKDIR /tmp/app/

VOLUME ["/tmp/app/"]
