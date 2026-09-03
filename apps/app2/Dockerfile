# Stage 0, "build-stage", based on Node.js, to build and compile the frontend
FROM nginxinc/nginx-unprivileged:1.31.0-alpine AS build-stage

WORKDIR /app/frontend

RUN echo $BUILD_VERSION > build-version.txt

