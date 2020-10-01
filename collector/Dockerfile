FROM ubuntu:18.04

ENV HW /home/hw
#RUN mkdir -p "$HW"
WORKDIR $HW

RUN apt-get update && apt-get install -y default-jdk git maven \
&& git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git \
&& mvn package -f ./boxfuse-sample-java-war-hello

