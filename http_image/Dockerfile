# My HTTP Docker image
# Version 1

# Pull the CentOS 7.2 image from the Docker Hub registry
FROM centos:7

LABEL author="Nam Nguyen Hoai"
USER root

# Update packages list and install some useful tools
# RUN yum update -y

# Add the httpd package
RUN yum install -y httpd

# Clean the yum cache
RUN yum clean all

# Set the Web Server name
RUN echo ServerName apache.example.com >> /etc/httpd/conf/httpd.conf

COPY index.html /var/www/html/

CMD [ "/usr/sbin/httpd", "-DFOREGROUND" ]   