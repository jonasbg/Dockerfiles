FROM alpine:latest

LABEL MAINTAINER="Jonas Bo Grimsgaard - jonas.bo.grimsgaard@nhn.no"

WORKDIR /bin
RUN apk --no-cache add curl
RUN curl -fsSL -o https://get.helm.sh/helm-v3.8.0-linux-amd64.tar.gz \
  && tar xvf helm-v3.8.0-linux-amd64.tar.gz \
  && mv linux-amd64/helm /bin/helm \
  && rm -rf linux-amd64 \
  && helm version
