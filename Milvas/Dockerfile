FROM nvidia/cuda:11.7.1-devel-ubuntu22.04

WORKDIR /work

RUN apt-get update && apt-get install -y \
    python3-pip \ 
    sudo \
    wget \
    git \
    build-essential \
    file \
    curl

RUN ln -s /usr/bin/python3.10 /usr/bin/python

ADD ./requirements.txt /work/requirements.txt

RUN pip3 install --upgrade pip
RUN pip3 install -r requirements.txt