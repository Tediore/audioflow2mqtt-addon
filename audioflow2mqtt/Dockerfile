ARG BUILD_FROM
FROM $BUILD_FROM

ADD audioflow2mqtt.py /

RUN apk add --no-cache python3
RUN python3 -m ensurepip
RUN pip3 install setuptools paho.mqtt requests pyyaml

CMD [ "python3", "./audioflow2mqtt.py" ]
