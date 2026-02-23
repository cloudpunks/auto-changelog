FROM ghcr.io/cloudpunks/alpine:3.19@sha256:86c4ac170ab7967cbae7ef1ccc82d3a871a81410c25496d468274611c35540e5
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
