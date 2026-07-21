FROM ghcr.io/cloudpunks/alpine:3.19@sha256:c52309fc12c2c1fe77a617f596399d68eef0c1772a75df80f06b169155dc345f
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
