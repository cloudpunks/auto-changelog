FROM ghcr.io/cloudpunks/alpine:3.19@sha256:69ad8cd708ea2323fdc112b732de748e7e7281a6a162f0f23c8de99c37e22f1c
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
