FROM ghcr.io/cloudpunks/alpine:3.19@sha256:cc94b01dc81fa3c23a8a4e203a24ba7017b0230c6de68e77a025fe11a5848888
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
