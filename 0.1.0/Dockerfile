FROM alpine:latest
MAINTAINER gavin zhou <gavin.zhou@gmail.com>

RUN apk update && apk add \
	ca-certificates \
	python \
	py-pip \
	&& rm -rf /var/cache/apk/*
RUN pip install httpie httpie-unixsocket httpie-oauth httpie-http2
