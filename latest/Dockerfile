FROM ghcr.io/cloudpunks/alpine:3.19@sha256:0e829901438c66c942eb00c6fcde06c68800ac883fac058c36e224dcc95af4a4
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
