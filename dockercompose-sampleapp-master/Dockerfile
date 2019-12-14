FROM gliderlabs/alpine:latest
MAINTAINER Junaid <example@example.com>
LABEL Description="Docker"

ADD . /sampleapp
WORKDIR /sampleapp
RUN apk-install python \
    python-dev \
    py-pip &&\
    pip install -r requirements.txt
CMD ["python", "app.py"]
