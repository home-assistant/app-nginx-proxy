ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.06.1
FROM $BUILD_FROM

# Setup base
RUN apk add --no-cache nginx openssl

# Copy data
COPY rootfs /

WORKDIR /

LABEL \
    org.opencontainers.image.title="Home Assistant App: NGINX Home Assistant SSL proxy" \
    org.opencontainers.image.description="An SSL/TLS proxy" \
    org.opencontainers.image.source="https://github.com/home-assistant/app-nginx-proxy" \
    org.opencontainers.image.licenses="Apache License 2.0"
