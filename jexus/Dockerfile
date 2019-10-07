FROM centos
EXPOSE 80
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' >/etc/timezone
WORKDIR /opt
RUN yum install -y wget
RUN wget https://www.linuxdot.net/down/jexus-6.1-x64.tar.gz
RUN tar zxvf jexus-6.1-x64.tar.gz
RUN rm -f jexus-6.1-x64.tar.gz
WORKDIR /var/www/default
CMD ["/opt/jexus/jwss"]
