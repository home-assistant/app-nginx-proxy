# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.10.3@sha256:880016115f356afc814398e17ba68a7ee66dfc1b4eaef09755ea2c9fa18ea481
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
