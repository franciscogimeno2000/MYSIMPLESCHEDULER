FROM ghcr.io/hassio-addons/base-python:16.1.0

RUN pip3 install Flask requests pytz psutil paho-mqtt 

COPY rootfs /

RUN find /etc/services.d -type f -exec chmod a+x {} \; \
    && find /simplescheduler -type f -name "*.sh" -exec chmod a+x {} \;
