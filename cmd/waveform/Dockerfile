FROM gliderlabs/alpine:3.4

COPY ./waveform .

ADD of-watchdog /usr/bin
RUN chmod +x /usr/bin/of-watchdog

ENV mode="afterburnstdio"
ENV fprocess="./waveform"

EXPOSE 8080
CMD ["of-watchdog"]