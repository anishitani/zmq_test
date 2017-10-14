FROM python:alpine
MAINTAINER André Nishitani <atoshio25@gmail.com>

RUN apk add --no-cache gcc musl-dev build-base g++ \
  && pip install pyzmq zmq \
  && mkdir /ws

ADD sub.py /ws

WORKDIR /ws

ENTRYPOINT [ "python","sub.py" ]
