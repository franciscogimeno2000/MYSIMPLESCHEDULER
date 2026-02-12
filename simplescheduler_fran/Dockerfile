FROM ghcr.io/hassio-addons/base-python:16.1.0

RUN pip3 install Flask requests pytz psutil paho-mqtt 

COPY rootfs /

RUN chmod a+x /etc/services.d/*/run \
 && chmod a+x /etc/cont-init.d/* 2>/dev/null || true
