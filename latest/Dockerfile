FROM ghcr.io/cloudpunks/alpine:3.19@sha256:e4f11c9c3cf8f425c168fce25fbe78e56f5f9099805113e64f591cd7349446a0
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
