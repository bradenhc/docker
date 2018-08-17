# Dockerfile
FROM centos
LABEL maintainer "Braden Hitchcock <developer.hitchcock@gmail.com>"

ENV HOME /root
ENV M2_HOME /usr/local/apache-maven
ENV M2 $M2_HOME/bin
ENV PATH $M2:$PATH

RUN yum -y --setopt=group_package_types=madatory,default,optional groupinstall "Development Tools" \
    && wget http://mirror.olnevhost.net/pub/apache/maven/maven-3/3.0.5/binaries/apache-maven-3.0.5-bin.tar.gz \
    && tar xvf apache-maven-3.0.5-bin.tar.gz \
    && mv apache-maven-3.0.5 /usr/local/apache-maven \
    && mvn -version

