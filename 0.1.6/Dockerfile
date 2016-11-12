FROM alpine:3.4
MAINTAINER gavin zhou <gavin.zhou@gmail.com>

RUN apk update && apk add \
  ca-certificates \
  python \
  py-pip \
  mysql-client wget git curl tar \
  && rm -rf /var/cache/apk/* \
  && pip install httpie httpie-unixsocket httpie-oauth httpie-http2 PyJWT uuid \
  && wget -q https://storage.googleapis.com/kubernetes-release/release/v1.4.5/bin/linux/amd64/kubectl -O /usr/bin/kubectl \
  && chmod +x /usr/bin/kubectl
