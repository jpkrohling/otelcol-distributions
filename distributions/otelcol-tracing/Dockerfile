FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-tracing /otelcol-tracing
COPY otelcol.yaml /etc/otelcol-tracing/config.yaml
ENTRYPOINT ["/otelcol-tracing"]
CMD ["--config", "/etc/otelcol-tracing/config.yaml"]
EXPOSE 4317
