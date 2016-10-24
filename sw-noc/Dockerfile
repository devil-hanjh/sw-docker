FROM ubuntu
MAINTAINER hanjh
RUN apt-get update 
RUN apt-get install -y snmp 
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
EXPOSE 2002
COPY swcollector /usr/local/swcollector
WORKDIR /usr/local/swcollector
ENTRYPOINT ["/usr/local/swcollector/falcon-swcollector"]

