FROM ghcr.io/cloudpunks/alpine:3.19@sha256:55cb12abfed844d599208f553b0f6d1447a3a57fc218528b79e7a53816939c35
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
