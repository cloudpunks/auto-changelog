FROM ghcr.io/cloudpunks/alpine:3.19@sha256:f6202196a100dc7be70afa420e87dcba8960921aa1b753685f493e139bacb002
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
