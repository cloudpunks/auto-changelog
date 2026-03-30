FROM ghcr.io/cloudpunks/alpine:3.19@sha256:83a3e9c20358b94316d0235f390bb1af21db48aa62a6f23578bfe7026beb82de
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
