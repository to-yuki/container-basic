# MyCustome Hello Container Image
FROM library/busybox:latest
ARG HELLO="Hello!"
ENV HELLO=Hello
LABEL IMAGE="MyCustome Hello Image"
WORKDIR /root

ADD ./src .
ADD ./src/archive.tar.gz .
COPY README.md .

RUN echo ${HELLO} > /root/hello
USER root
CMD cat /root/hello
