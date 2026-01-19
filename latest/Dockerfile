FROM ghcr.io/cloudpunks/alpine:3.19@sha256:896769e134761d2ecc93f25b6255a06024800e7c7805370deb956edc15468f69
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
