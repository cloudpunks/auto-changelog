FROM ghcr.io/cloudpunks/alpine:3.19@sha256:ebdad44cd1c0bdfb08fd9f9d5e2624df2dba262e11fa86515f676859ee3177e5
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
