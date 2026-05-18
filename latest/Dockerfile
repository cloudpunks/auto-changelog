FROM ghcr.io/cloudpunks/alpine:3.19@sha256:242e91d08b55de3a20b6782960d78d474850dc3c4e671fa9dc467469665e02ef
ENTRYPOINT [""]

# renovate: datasource=npm depName=auto-changelog
ENV AUTO_CHANGELOG_VERSION=2.4.0

RUN apk update && \
  apk upgrade && \
  apk add nodejs npm git && \
  npm install --global \
    auto-changelog@${AUTO_CHANGELOG_VERSION} && \
  rm -rf /var/cache/apk/*
