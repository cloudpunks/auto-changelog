FROM ghcr.io/cloudpunks/alpine:3.19@sha256:525f99b30906070a992f89edbd9efa74f38f9533612671cb14de3f580e9efee5
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
