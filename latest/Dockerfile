FROM ghcr.io/cloudpunks/alpine:3.19@sha256:f0d0e20158b4757ab2476ae46aa1df529253ad49d9a22446e5dc222aaf1870f8
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
