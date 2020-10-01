FROM tomcat

ENV HW /usr/local/tomcat/webapps
ENV WAR /home/hw/boxfuse-sample-java-war-hello
WORKDIR $HW

RUN cp $WAR/target/hello-1.0.war $HW

CMD ["catalina.sh", "run"]