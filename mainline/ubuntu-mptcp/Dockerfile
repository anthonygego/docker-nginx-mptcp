#
# NOTE: THIS DOCKERFILE IS GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY.
#
FROM nginx:1.23.3

RUN set -x \
    && apt-get update \
    && apt-get install --no-install-recommends --no-install-suggests -y mptcpize \
    && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/*

CMD ["mptcpize", "run", "nginx", "-g", "daemon off;"]
