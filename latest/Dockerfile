FROM ghcr.io/cloudpunks/alpine:3.19@sha256:17c393a33034e12ca4ba9a263e8c81358ae8fb3ecfc146f7de2f7ba10ef935b6
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
