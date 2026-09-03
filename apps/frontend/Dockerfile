# Stage 0, "build-stage", based on Node.js, to build and compile the frontend
FROM node:22.23.2-alpine AS build-stage

WORKDIR /app/frontend

RUN echo $BUILD_VERSION > build-version.txt



# Stage 1, based on Nginx, to have only the compiled app, ready for production with Nginx
FROM nginxinc/nginx-unprivileged:1.31.0-alpine3.23

FROM nginxinc/nginx-unprivileged:1.31.0-alpine

RUN echo "hello world"

EXPOSE 8080
