FROM ghcr.io/cloudpunks/alpine:3.19@sha256:b7fa9c5a5990efcb67547792780480668730c2a72ded5b2bd123effdcad7174d
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.6.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
