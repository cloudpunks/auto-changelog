FROM ghcr.io/cloudpunks/alpine:3.19@sha256:6c15ca94ffea2f7b013f38a612347c071544a7a497f6e561c44ae9b544b00994
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
