FROM jenkinsci/blueocean

USER root

ARG DOCKER_COMPOSE_VERSION=1.28.4

RUN apk update \
    && apk add --no-cache --update make py3-pip \
    \
    && apk add --no-cache musl-dev cargo\
    && apk add --no-cache --update --virtual .docker-compose-deps \
      gcc \
      libc-dev \
      libffi-dev \
      python3-dev \
      openssl-dev \
    \
    && pip install -U docker-compose==${DOCKER_COMPOSE_VERSION} \
    \
    && apk del .docker-compose-deps \
    && rm -rf `find / -regex '.*\.py[co]' -or -name apk`

USER jenkins
