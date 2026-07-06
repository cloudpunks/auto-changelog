FROM ghcr.io/cloudpunks/alpine:3.19@sha256:381202025a6f09a9525ed978405d93898fb8c490f6dcc7dbd3ce3a0adbcffccf
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
