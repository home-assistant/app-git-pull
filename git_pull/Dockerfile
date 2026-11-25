# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.11.1@sha256:5021aac8a4b7f2a1397e23a9749dfe9f736463ffa471df6b200216c68d530fe6
FROM $BUILD_FROM

# Setup base
RUN apk add --no-cache jq curl git openssh-client

# Copy data
COPY data/run.sh /

CMD [ "/run.sh" ]

LABEL \
    org.opencontainers.image.title="Home Assistant App: Git pull" \
    org.opencontainers.image.description="Simple git pull to update the local configuration" \
    org.opencontainers.image.source="https://github.com/home-assistant/app-git-pull" \
    org.opencontainers.image.licenses="Apache License 2.0"
