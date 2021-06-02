FROM ubuntu:20.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt install default-jdk  maven git -y
RUN mkdir -p /opt/test/boxfuse 
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /opt/test/boxfuse/
RUN mvn -f /opt/test/boxfuse/pom.xml package