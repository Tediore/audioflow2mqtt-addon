FROM alpine:3

ADD audioflow2mqtt.py /

RUN apk add --no-cache python3
RUN python3 -m ensurepip
RUN pip3 install setuptools aiomqtt pyyaml httpx

CMD [ "python3", "./audioflow2mqtt.py" ]
