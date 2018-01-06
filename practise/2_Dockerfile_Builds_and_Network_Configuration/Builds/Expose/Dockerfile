#  This image is based on cento7 and will start apache service
FROM centos:latest
MAINTAINER sam943@gmail.com

RUN yum update -y
RUN yum install -y httpd net-tools dnsmasq telnet

RUN echo "Ths is custom index file during the image build" > /var/www/html/index.hmtl
RUN echo "ServerName localhost" >> /etc/httpd/conf/httpd.conf

EXPOSE 80

ENTRYPOINT systemctl enable dnsmasq 
ENTRYPOINT systemctl enable httpd
ENTRYPOINT apachectl "-D FOREGROUND"
