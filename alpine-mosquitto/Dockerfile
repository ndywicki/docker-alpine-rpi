FROM privateport/alpine-rpi:3.3
MAINTAINER ndywicki, https://github.com/ndywicki/docker-alpine-rpi

RUN apk add --update mosquitto mosquitto-clients && \
mkdir /work && chown nobody /work

VOLUME ["/work"]
WORKDIR /work

USER nobody

EXPOSE 1883

ENTRYPOINT ["mosquitto"]
