FROM ghcr.io/cloudpunks/alpine:3.19@sha256:ba6b0be1afd01f50a9f1d1f1702a7182fb9684e12665f1475279400c9f8b4a7a
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
