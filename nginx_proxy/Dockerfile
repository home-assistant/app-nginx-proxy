# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.11.1@sha256:5021aac8a4b7f2a1397e23a9749dfe9f736463ffa471df6b200216c68d530fe6
FROM $BUILD_FROM

# Setup base
RUN apk add --no-cache "nginx>=1.30.7" openssl

# Copy data
COPY rootfs /

WORKDIR /

LABEL \
    org.opencontainers.image.title="Home Assistant App: NGINX Home Assistant SSL proxy" \
    org.opencontainers.image.description="An SSL/TLS proxy" \
    org.opencontainers.image.source="https://github.com/home-assistant/app-nginx-proxy" \
    org.opencontainers.image.licenses="Apache License 2.0"
