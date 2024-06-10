FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-loadbalancer /otelcol-loadbalancer
COPY config.yaml /etc/otelcol-loadbalancer/config.yaml
ENTRYPOINT ["/otelcol-loadbalancer"]
CMD ["--config", "/etc/otelcol-loadbalancer/config.yaml"]
EXPOSE 4317
