FROM alpine:3

ADD audioflow2mqtt.py /

RUN apk add --no-cache python3
RUN apk add py3-pip
RUN pip install --break-system-packages setuptools aiomqtt pyyaml httpx

CMD [ "python3", "./audioflow2mqtt.py" ]
