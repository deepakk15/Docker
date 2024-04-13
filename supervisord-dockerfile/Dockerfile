FROM centos:7
RUN yum update -y && yum install httpd epel-release -y && yum install -y supervisor
RUN mkdir -p /var/log/supervisor
RUN chown -R root:root /var/log/supervisor
COPY supervisord.conf /etc/supervisord.conf
EXPOSE 80
CMD ["/usr/bin/supervisord", "-c", "/etc/supervisord.conf"]