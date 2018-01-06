#Dockerfile based on the latest Centos 7 imae - non-privileged user entry
FROM centos:latest
MAINTAINER sam943@gmail.com

RUN echo "Export 192.168.0.0/24" >> /etc/exports.list

RUN useradd -ms /bin/bash user

RUN yum update -y
RUN yum install -y net-tools wget

# RUN cd - && wget "url to download java rpm from internet"
# RUN yum localinstall -y "java_package"

User user
RUN echo "export JAVA_HOME=/usr/java/jdk1.7" >> /home/user/.bashrc

ENV JAVA_BIN /usr/java/jdk1.7
