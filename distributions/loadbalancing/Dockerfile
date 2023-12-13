FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY loadbalancing /loadbalancing
COPY otelcol.yaml /etc/loadbalancing/config.yaml
ENTRYPOINT ["/loadbalancing"]
CMD ["--config", "/etc/loadbalancing/config.yaml"]
EXPOSE 4317
