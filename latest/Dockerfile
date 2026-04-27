FROM ghcr.io/cloudpunks/alpine:3.19@sha256:051c3b98a6c471f09ded2bb4834b814404f6ff6a842e780d8bec1bd5e6bc52ce
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
