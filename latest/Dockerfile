FROM ghcr.io/cloudpunks/alpine:3.24@sha256:bacb232473dfec7a700675b3e139e3944ad3fb26f27e59a63b86962dd7e279af
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.6.1

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
