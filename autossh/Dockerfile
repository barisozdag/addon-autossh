ARG BUILD_FROM=ghcr.io/hassio-addons/base/aarch64:15.0.3
# hadolint ignore=DL3006
FROM $BUILD_FROM

# Set shell
SHELL ["/bin/bash", "-o", "pipefail", "-c"]

# Setup base system
ARG BUILD_ARCH=aarch64

ENV LANG C.UTF-8

RUN apk add --no-cache \
  tzdata=2023d-r0 \
  jq=1.7.1-r0 \
  openssh=9.6_p1-r0 \
  vim=9.0.2127-r0 \
  curl=8.5.0-r0 \
  autossh=1.4g-r3

# Copy root filesystem
COPY rootfs /

# Build arguments
ARG BUILD_ARCH
ARG BUILD_DATE
ARG BUILD_DESCRIPTION
ARG BUILD_NAME
ARG BUILD_REF
ARG BUILD_REPOSITORY
ARG BUILD_VERSION

# Labels
LABEL \
    io.hass.name="${BUILD_NAME}" \
    io.hass.description="${BUILD_DESCRIPTION}" \
    io.hass.arch="${BUILD_ARCH}" \
    io.hass.type="addon" \
    io.hass.version=${BUILD_VERSION} \
    maintainer="Barış Özdağ" \
    org.opencontainers.image.title="${BUILD_NAME}" \
    org.opencontainers.image.description="${BUILD_DESCRIPTION}" \
    org.opencontainers.image.vendor="barisozdag's Personal Home Assistant Add-ons" \
    org.opencontainers.image.authors="Barış Özdağ" \
    org.opencontainers.image.licenses="MIT" \
    org.opencontainers.image.url="https://github.com/barisozdag/addon-autossh" \
    org.opencontainers.image.source="https://github.com/${BUILD_REPOSITORY}" \
    org.opencontainers.image.documentation="https://github.com/${BUILD_REPOSITORY}/blob/main/README.md" \
    org.opencontainers.image.created=${BUILD_DATE} \
    org.opencontainers.image.revision=${BUILD_REF} \
    org.opencontainers.image.version=${BUILD_VERSION}
