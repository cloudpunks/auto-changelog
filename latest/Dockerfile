FROM ghcr.io/cloudpunks/alpine:3.24@sha256:f735e3f0ae5b8ab423c6467079a33c38e2700eab720cc676f5a330b44eb9d05d
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.6.1

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
