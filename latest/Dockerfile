FROM ghcr.io/cloudpunks/alpine:3.19@sha256:4d9e4caea8b63ce9d1648e33e2a861ad74c9f357d44a67f712344a320300de85
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
