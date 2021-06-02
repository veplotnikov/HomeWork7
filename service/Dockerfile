FROM ubuntu:20.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update \
    apt-get install wget \
    mkdir /opt/tomcat \
    wget https://www-eu.apache.org/dist/tomcat/tomcat-9/v9.0.46/bin/apache-tomcat-9.0.46.tar.gz -P /tmp \
    tar -xf /tmp/apache-tomcat-9.0.46.tar.gz -C /opt/tomcat/
    ln -s /opt/tomcat/apache-tomcat-9.0.46 /opt/tomcat/latest \
    sh -c 'chmod +x /opt/tomcat/latest/bin/*.sh' 

CMD ["/opt/tomcat/latest/bin/catalina.sh", "run"]