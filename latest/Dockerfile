FROM ghcr.io/cloudpunks/alpine:3.19@sha256:25b5279743053a31300d52aeea02743c57b9e613fb67d2a87628383ba4e3685b
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
