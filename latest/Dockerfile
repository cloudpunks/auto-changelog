FROM ghcr.io/cloudpunks/alpine:3.19@sha256:5dddb7594431a9c5db49854fa3c3e10a99aedaffa053f62f7fc77e620246bfed
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
