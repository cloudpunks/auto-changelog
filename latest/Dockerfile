FROM ghcr.io/cloudpunks/alpine:3.19@sha256:b6326bdeb79bd21dfe730daaa67c16598acf9f345590781bcaad5b12459f07ac
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
