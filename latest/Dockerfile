FROM ghcr.io/cloudpunks/alpine:3.19@sha256:14a2088af05369ebd82c3a80e8159f2b7dc6aebdcbdb00c65e1ed9470525e91a
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
