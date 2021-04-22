# SL Container
FROM docker.io/library/centos

LABEL name=SL
ENV name=SL

RUN yum install -y epel-release && \
    yum install -y sl && \
    yum clean all                                                                                                                       
USER root
CMD ["/usr/bin/sl"]
