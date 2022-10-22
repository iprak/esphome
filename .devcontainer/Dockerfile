FROM python:3.8

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        git \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/*

RUN pip install --upgrade esphome esptool platformio

WORKDIR /workspace