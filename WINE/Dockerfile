FROM debian:buster-slim

RUN dpkg --add-architecture i386 && apt-get update

RUN apt-get install -y wine

ENTRYPOINT ["/usr/bin/wine"]
CMD ["--version"]
