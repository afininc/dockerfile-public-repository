FROM alpine:3.18
ENV LANG C.UTF-8

LABEL name="node20-jre8-alpine-base"
LABEL maintainer="AFIN I&C <hanu@a-fin.co.kr>"

ENV JAVA_ALPINE_VERSION 8.392.08-r1

ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk/jre
ENV PATH $PATH:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin


RUN set -x \
	&& apk add --no-cache \
    openjdk8="$JAVA_ALPINE_VERSION"

RUN apk add  --no-cache  --repository http://dl-cdn.alpinelinux.org/alpine/edge/main --allow-untrusted \
    nodejs-current \
    npm \
    yarn