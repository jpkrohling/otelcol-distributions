FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-otlp /otelcol-otlp
COPY otelcol.yaml /etc/otelcol-otlp/config.yaml
ENTRYPOINT ["/otelcol-otlp"]
CMD ["--config", "/etc/otelcol-otlp/config.yaml"]
EXPOSE 4317
