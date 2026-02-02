FROM ghcr.io/cloudpunks/alpine:3.19@sha256:81884e08538321c6bc893c2f06739bfbb35470908d1f0e59bf493fd1bed7d26d
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
