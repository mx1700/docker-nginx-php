# Version: 0.0.1
FROM centos:7
MAINTAINER lizhaoguang "lizhaoguang@dangdang.com"
ENV REFRESHED_AT 2016-04-16

RUN yum -y update
RUN yum install -y epel-release
RUN yum -y update

RUN yum install -y nginx
RUN mkdir /app
WORKDIR /app
ADD nginx.conf /etc/nginx/nginx.conf

CMD nginx -g "daemon off;"
EXPOSE 80

