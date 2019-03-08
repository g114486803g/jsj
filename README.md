# base image
FROM centos7.6

# MAINTAINER
MAINTAINER json_hc@1231.com



# running required command
RUN yum install -y gcc gcc-c++ glibc make autoconf openssl openssl-devel 
RUN yum install -y  pcre pcre-devel
RUN useradd -M -s /sbin/nologin nginx

EXPOSE 80
