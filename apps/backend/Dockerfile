FROM node:22.14.0-alpine AS build-stage

USER node

RUN mkdir -p /home/node/app/backend
RUN mkdir -p /home/node/validation


WORKDIR /home/node/app/backend

RUN echo "hello world"

FROM node:22.14.0-alpine

USER node

RUN mkdir -p /home/node/app/backend
RUN mkdir -p /home/node/validation

WORKDIR /home/node/app/backend

ARG BUILD_VERSION=<unknown>
RUN echo $BUILD_VERSION > build-version.txt

EXPOSE 4000

CMD [ "node", "./build/index.js" ]
