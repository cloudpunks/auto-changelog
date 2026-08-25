FROM ghcr.io/cloudpunks/alpine:3.24@sha256:c05a9a0ce1b3d9e2f216b0024f499a562977cfa67174c20e9f9a19dee301ad04
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.6.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
