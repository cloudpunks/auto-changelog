FROM ghcr.io/cloudpunks/alpine:3.24@sha256:9482e5bfa69beff273ddfc00004f101cb03760c7d98d0a727377fc30f7aff66a
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
