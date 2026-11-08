FROM ghcr.io/cloudpunks/alpine:3.24@sha256:3a7fd091452d064e70973d5d995e1fe53557064a215512d9f6221ac83d76e301
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
