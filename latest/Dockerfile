FROM ghcr.io/cloudpunks/alpine:3.24@sha256:7cb29c630a04ad696336943dc35fa54e1750a6fb29e99bab34dc7af644f4e900
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.7.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
