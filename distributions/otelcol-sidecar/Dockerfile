FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-sidecar /otelcol-sidecar
COPY otelcol.yaml /etc/otelcol-sidecar/config.yaml
ENTRYPOINT ["/otelcol-sidecar"]
CMD ["--config", "/etc/otelcol-sidecar/config.yaml"]
EXPOSE 4317
