FROM ghcr.io/cloudpunks/alpine:3.19@sha256:d8b7370e1237529c1f919ae2aaac09b30b0bb1fb95da94b6020231d85efabb7a
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
