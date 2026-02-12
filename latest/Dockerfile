FROM ghcr.io/cloudpunks/alpine:3.19@sha256:6aadf3a197fcbd87a3d1cf01e5bb3773e4e5343ec5ca0a09ea84b69ea800791e
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
