FROM ghcr.io/cloudpunks/alpine:3.19@sha256:b69baaaddb2ce4ccf0ccb35aba6efd5a220014543d16519beb8fe7597967c62d
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
