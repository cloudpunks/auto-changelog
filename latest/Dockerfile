FROM ghcr.io/cloudpunks/alpine:3.24@sha256:e86358e09c99af83800967323e85560c8c3d91f9cf540339eae68d814c660012
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
