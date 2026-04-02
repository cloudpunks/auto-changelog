FROM ghcr.io/cloudpunks/alpine:3.19@sha256:a3bb22a58ab667dcfcfd891fa0d89ac5df41edb41fb7794c776568d61ee9706b
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
