FROM ghcr.io/cloudpunks/alpine:3.19@sha256:2363ec3b5cbeddb1238fc15b50864539d6064ded6df5c84ce036cf33a7deb6e0
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
