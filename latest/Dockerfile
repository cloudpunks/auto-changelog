FROM ghcr.io/cloudpunks/alpine:3.24@sha256:91e446169b936cbc2d4a9a269181f583f466518dc6a80c6baaa3d28a212a5660
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
