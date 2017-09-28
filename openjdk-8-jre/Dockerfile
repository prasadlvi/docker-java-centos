FROM centos:7

MAINTAINER nimmis <brett.wooldridge@gmail.com>

RUN yum update -y && \
yum install -y wget && \
yum install -y java-1.8.0-openjdk && \
yum install -y iproute && \
yum clean all

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]

