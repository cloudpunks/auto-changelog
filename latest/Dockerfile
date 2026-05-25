FROM ghcr.io/cloudpunks/alpine:3.19@sha256:6c6fc49634697a283ba3190d7b1949a3853b39a1eed4a981701daf95ca0969c3
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
