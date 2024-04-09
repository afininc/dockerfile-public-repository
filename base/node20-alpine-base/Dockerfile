FROM alpine:3.18
ENV LANG C.UTF-8

LABEL name="node20-alpine-base"
LABEL maintainer="AFIN I&C <hanu@a-fin.co.kr>"

RUN apk add  --no-cache  --repository http://dl-cdn.alpinelinux.org/alpine/edge/main --allow-untrusted \
    nodejs-current \
    npm \
    yarn