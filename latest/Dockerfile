FROM ghcr.io/cloudpunks/alpine:3.19@sha256:1137281fed3287438ce085bb5abde5b05f20b303d6b16e5ae62ea3bbe5737ff2
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
