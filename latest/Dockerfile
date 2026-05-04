FROM ghcr.io/cloudpunks/alpine:3.19@sha256:f9a812ca3dd80247fa3915bb24eb00bf7453a2f189207a55045e47308ed3147e
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
