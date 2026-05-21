FROM ghcr.io/cloudpunks/alpine:3.19@sha256:f84f45b86829d7e7ca097cf0042b12380eb2a8f8d5f69fd1e71410c214d35fb5
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
