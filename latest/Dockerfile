FROM ghcr.io/cloudpunks/alpine:3.19@sha256:dac83fdf5f27838c3fe4c90b3f6eb262752db70de97e570681a0d6d02e411759
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
