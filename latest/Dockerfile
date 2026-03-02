FROM ghcr.io/cloudpunks/alpine:3.19@sha256:69022bf9cf0b23fa705a2da7b8c9527cf4388eea5ec982d25f21e1d94e8bec66
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
