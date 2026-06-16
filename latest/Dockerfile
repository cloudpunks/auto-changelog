FROM ghcr.io/cloudpunks/alpine:3.19@sha256:d72340bcdd42a4bf7c8f68b292a6d140eeb7c6b6ccd813c79a8a9ffd793729d0
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
