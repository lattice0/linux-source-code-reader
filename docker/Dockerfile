FROM ubuntu:focal

RUN apt-get update -o Acquire::Retries=30 \ 
&& DEBIAN_FRONTEND=noninteractive apt-get install -o Acquire::Retries=30 -y --no-install-recommends \
clang gcc build-essential wget git python unzip ca-certificates

WORKDIR /home/project

RUN mkdir linux && cd linux && wget https://github.com/torvalds/linux/archive/master.zip && unzip master.zip