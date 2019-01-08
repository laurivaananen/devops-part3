FROM ubuntu:16.04

ENV LC_ALL=C.UTF-8

WORKDIR /app

RUN apt-get update && apt-get install -y \
    python2.7 ffmpeg curl && \
    curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py && \
    python2.7 get-pip.py &&\
    pip install -U yle-dl && \
    apt-get purge -y --auto-remove curl  && \
    rm -rf /var/lib/apt/lists/* && \
    rm get-pip.py

ENTRYPOINT ["yle-dl"]