FROM arm64v8/ubuntu:20.04

RUN apt-get update && apt-get install -y --no-install-recommends apt-utils

RUN apt-get install openjdk-8-jre-headless -y

RUN apt-get install curl tar vim -y

RUN apt-get install python -y

RUN mkdir -p /home/cc
ADD storm /home/cc/storm

WORKDIR /home/cc/storm

ADD configure.sh /
