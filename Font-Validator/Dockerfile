FROM ubuntu:16.04

ARG FONT_VALIDATOR_VERSION=2.1.1

RUN apt-get update -qy && apt-get install -y curl

RUN curl -L https://github.com/HinTak/Font-Validator/releases/download/FontVal-${FONT_VALIDATOR_VERSION}-py/Linux.FontVal-${FONT_VALIDATOR_VERSION}-py-ubuntu-16.04-x64.tgz | tar zxf - && \
    mv FontVal-${FONT_VALIDATOR_VERSION}-py-ubuntu-16.04-x64/FontValidator-ubuntu-16.04-x64 /usr/local/bin

ENTRYPOINT ["/usr/local/bin/FontValidator-ubuntu-16.04-x64"]
CMD ["-version"]
