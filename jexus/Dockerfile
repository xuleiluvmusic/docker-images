FROM centos
EXPOSE 80
RUN /bin/cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' >/etc/timezone
WORKDIR /opt
COPY jexus/ ./jexus
WORKDIR /var/www/default
CMD ["/opt/jexus/jwss"]
