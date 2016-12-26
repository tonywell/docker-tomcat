FROM 192.168.50.84:5000/tonywell/jdk:7-alpine

MAINTAINER tonywell "tongwei1985@gmail.com"

ARG TOMCAT_MAJOR_VERSION=7
ARG TOMCAT_UPDATE_VERSION=0
ARG TOMCAT_BUILD_NUMBER=73

RUN cd /tmp && \
    wget http://mirror.bit.edu.cn/apache/tomcat/tomcat-${TOMCAT_MAJOR_VERSION}/v${TOMCAT_MAJOR_VERSION}.${TOMCAT_UPDATE_VERSION}.${TOMCAT_BUILD_NUMBER}/bin/apache-tomcat-${TOMCAT_MAJOR_VERSION}.${TOMCAT_UPDATE_VERSION}.${TOMCAT_BUILD_NUMBER}.tar.gz && \
    mkdir -p /home/tomcat && \
    tar -xzf apache-tomcat-${TOMCAT_MAJOR_VERSION}.${TOMCAT_UPDATE_VERSION}.${TOMCAT_BUILD_NUMBER}.tar.gz -C /home/tomcat && \
    mv /home/tomcat/apache-tomcat-${TOMCAT_MAJOR_VERSION}.${TOMCAT_UPDATE_VERSION}.${TOMCAT_BUILD_NUMBER} /home/tomcat/tomcat-${TOMCAT_MAJOR_VERSION} && \    
    rm -rf /tmp/*

 
 
