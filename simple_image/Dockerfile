FROM centos:7

LABEL author="Nam Nguyen Hoai"

WORKDIR /opt

ADD hello-world.sh .

ARG IMAGE_VERSION

ENV IMAGE_VERSION v1.0

# RUN echo "Start building a new images"
RUN echo ${IMAGE_VERSION} > /root/version.txt

# EXPOSE 5000

CMD [ "sleep", "1000" ]
