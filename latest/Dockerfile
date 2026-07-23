FROM ghcr.io/cloudpunks/alpine:3.19@sha256:adf2261265592496a94c4211425942d4463a96ac7e2365d267094b68d2f3211f
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
