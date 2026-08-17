FROM ghcr.io/cloudpunks/alpine:3.19@sha256:9d43ef19d66c44aae64c31b64ed67e40d0a74e2a334285ecd82d29a64dd7fcf5
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
