FROM ghcr.io/cloudpunks/alpine:3.19@sha256:3e9f9be13ba76780b332965d493b83ca33c5859b916d0d95413a84dae340e272
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
