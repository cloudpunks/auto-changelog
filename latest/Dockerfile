FROM ghcr.io/cloudpunks/alpine:3.19@sha256:59ae5ffc21e78c2df65ef017296cb3fc49a0cd61e443606704de7e4279651cc1
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
