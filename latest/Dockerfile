FROM ghcr.io/cloudpunks/alpine:3.19@sha256:4ed896330dc4e175087c3d807985cb8c562bfe79229b37998cc8047096719de4
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
