FROM centos:7

MAINTAINER nimmis <brett.wooldridge@gmail.com>

RUN yum update -y && \
    yum install -y wget && \
    yum install -y java-1.8.0-openjdk && \
    yum install -y iproute && \
    yum install -y openssl098e && \
    yum install -y postgresql && \
    yum install -y unzip && \
    yum clean all && \
    ln -s /usr/lib64/libexpat.so.1 /usr/lib64/libexpat.so.0

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["bash"]
