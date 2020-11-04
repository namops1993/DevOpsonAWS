FROM centos:7

LABEL author="Nam Nguyen Hoai"
WORKDIR /root
ADD app.py .

COPY requirements.txt .
ARG IMAGE_VERSION
ENV IMAGE_VERSION v1.0
RUN yum update -y && \
    yum install -y epel-release && \
    yum install -y python-pip

RUN pip install -r requirements.txt
RUN echo ${IMAGE_VERSION} > /root/version.txt

VOLUME /var/log
EXPOSE 5000

CMD [ "python", "app.py" ]
