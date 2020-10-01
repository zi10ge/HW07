FROM ubuntu:18.04

ENV WAR /home/war
ENV SS /home/SS
RUN mkdir -p "$SS"
RUN mkdir -p "$WAR"
WORKDIR $SS

RUN apt-get update && apt-get install -y default-jdk git maven \
&& git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git \
&& mvn package -f ./boxfuse-sample-java-war-hello

RUN cp "$SS/boxfuse-sample-java-war-hello/target/hello-1.0.war" "$WAR/hello-1.0.war"
