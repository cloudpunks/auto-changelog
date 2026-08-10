FROM ghcr.io/cloudpunks/alpine:3.19@sha256:f53d30f105636aff5d02554ded8d8a2b23129224bfe8cbf0fc702649b386f57e
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
