FROM ghcr.io/cloudpunks/alpine:3.19@sha256:8fc1fa1305afb6acb25274d28e875806c06df5922e8c940a6b85bb1f5d5dc8e6
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
