FROM ghcr.io/cloudpunks/alpine:3.19@sha256:a9b1d4ca639285375a122f3568a9684b076c66daac7477e1d8c8844e81561aa0
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
