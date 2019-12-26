FROM ubuntu:16.04

RUN set -eux; \
    apt-get update; \
    apt-get install -y --no-install-recommends \
        ca-certificates \
        cargo \
        libpq-dev \
        ; \
    cargo --version; \
    rustc --version; \
    apt-get remove -y --auto-remove \
        ; \
    rm -rf /var/lib/apt/lists/*;

WORKDIR /src

VOLUME /out
