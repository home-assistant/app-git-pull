# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.10.1@sha256:992dc6a5727b97a30da8dd259b489739299c324407557df540165e2f0dbb7763
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
