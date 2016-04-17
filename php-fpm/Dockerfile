# Version: 0.0.1
FROM centos:7
MAINTAINER lizhaoguang "lizhaoguang@dangdang.com"
ENV REFRESHED_AT 2016-04-16

RUN yum -y update
RUN yum install -y epel-release
RUN yum -y update

RUN yum install -y php php-fpm composer
# php 5.4 版本过低
RUN mkdir /app
WORKDIR /app
ADD etc /etc

CMD php-fpm --fpm-config /etc/php-fpm.conf
EXPOSE 9000

# CMD php -S 0.0.0.0:8080
# EXPOSE 8080


