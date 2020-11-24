# MyPersistent Container Image
FROM library/busybox:latest
ARG HELLO="Hello!"
ENV HELLO=Hello
LABEL IMAGE="MyCustome Hello Image"

RUN adduser user01 --disabled-password && \ 
    mkdir /data && \ 
    chmod 775 /data && \ 
    chown -R user01:user01 /data

VOLUME /data
WORKDIR /data

USER user01
CMD /bin/sh
