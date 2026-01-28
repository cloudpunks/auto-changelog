FROM ghcr.io/cloudpunks/alpine:3.19@sha256:2c235eb709a179145331624ded029968fb0db510f61be53d5cc89a1953734cfe
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
