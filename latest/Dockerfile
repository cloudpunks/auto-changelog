FROM ghcr.io/cloudpunks/alpine:3.24@sha256:6c38f325099639d323a06b213d58fb8b13a9d84b8ef33a7008dba10bbef86246
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
