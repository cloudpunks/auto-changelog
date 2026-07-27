FROM ghcr.io/cloudpunks/alpine:3.19@sha256:3b8f511db2c0caf9795a757a7ce787549403708202c136aeb096dbe38aa461ba
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
