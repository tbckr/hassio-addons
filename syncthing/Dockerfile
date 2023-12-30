
ARG BUILD_FROM=ghcr.io/home-assistant/amd64-base:3.19
FROM $BUILD_FROM

COPY rootfs /

# renovate: datasource=repology depName=alpine_3_19/syncthing versioning=loose
ENV SYNCTHING_VERSION="1.27.1-r1"
RUN apk add --no-cache --repository=https://dl-cdn.alpinelinux.org/alpine/edge/community \
    "syncthing=${SYNCTHING_VERSION}"
