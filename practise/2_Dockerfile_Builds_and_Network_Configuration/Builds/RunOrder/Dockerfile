#Dockerfile based on the latest Centos 7 imae - non-privileged user entry
FROM centos:latest
MAINTAINER sam943@gmail.com

RUN echo "Export 192.168.0.0/24" >> /etc/exports.list

RUN useradd -ms /bin/bash user
USER user

# RUN command used to execute the the command at runtime and becomes part of the image

