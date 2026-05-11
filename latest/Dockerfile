FROM ghcr.io/cloudpunks/alpine:3.19@sha256:cde5f5b760ac4b3afb5dcb46924a2144a33c05d33b0e7e0d4fb4bf61ae444bf2
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
