FROM ghcr.io/cloudpunks/alpine:3.19@sha256:4d01c8e190affb14bd1789df7f96e82206a5b3c6c3877b755533cc84ab73d46e
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
