FROM ghcr.io/cloudpunks/alpine:3.19@sha256:cc09c815f6d8ec9f5cf945c7d7ec9630755ffa9e312d47ab6fd7a82f68a0ae04
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
