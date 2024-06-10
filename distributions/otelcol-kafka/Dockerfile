FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-kafka /otelcol-kafka
COPY config.yaml /etc/otelcol-kafka/config.yaml
ENTRYPOINT ["/otelcol-kafka"]
CMD ["--config", "/etc/otelcol-kafka/config.yaml"]
EXPOSE 4317
