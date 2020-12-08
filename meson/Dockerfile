FROM ubuntu:18.04

ARG PROXY
ENV HTTP_PROXY=${PROXY}
ENV HTTPS_PROXY=${PROXY}
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y --no-install-recommends \
        build-essential \
        git \
        bash-completion

RUN useradd -u 1000 -m -s /bin/bash ubuntu

USER ubuntu
WORKDIR /home/ubuntu
