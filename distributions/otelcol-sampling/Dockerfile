FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-sampling /otelcol-sampling
COPY config.yaml /etc/otelcol-sampling/config.yaml
ENTRYPOINT ["/otelcol-sampling"]
CMD ["--config", "/etc/otelcol-sampling/config.yaml"]
EXPOSE 4317
