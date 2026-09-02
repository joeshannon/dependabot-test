# Stage 0, "build-stage", based on Node.js, to build and compile the frontend
FROM node:22.14.0-alpine AS build-stage

ARG ORCID_REDIRECT=
ARG BUILD_VERSION=<unknown>


WORKDIR /app/frontend

RUN echo $BUILD_VERSION > build-version.txt



# Stage 1, based on Nginx, to have only the compiled app, ready for production with Nginx
FROM nginxinc/nginx-unprivileged:alpine3.23

RUN echo "hello world"

EXPOSE 8080
