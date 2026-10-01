FROM ghcr.io/cloudpunks/alpine:3.24@sha256:1ff90666d642910c31f8643e00b9fae907e95f500a82a2e1c2becc96b6e9c3e9
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
