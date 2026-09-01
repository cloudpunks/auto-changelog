FROM ghcr.io/cloudpunks/alpine:3.24@sha256:dac428a9b6d3aa41809f34a428ee8550a4f2ba99d82c75e9689d4cf055fc2e78
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.6.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
