FROM centos:7

MAINTAINER prasad <prasad@lvi.co.jp>

RUN yum update -y && \
    yum install -y wget && \
    wget https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz && \
    tar xzf openjdk-11.0.1_linux-x64_bin.tar.gz -C /usr/local && \
    cd /usr/local/jdk-11.0.1 && \
    alternatives --install /usr/bin/java java /usr/local/jdk-11.0.1/bin/java 2 && \
    alternatives --set java /usr/local/jdk-11.0.1/bin/java && \
    yum install -y freetype && \
    yum install -y urw-fonts && \
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
