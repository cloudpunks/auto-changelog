FROM ghcr.io/cloudpunks/alpine:3.24@sha256:1aa42e6acf3d3ba10b3edd39469425e03cc3edcc4e25b387ac466ccbd08fa727
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
