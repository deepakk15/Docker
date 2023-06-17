FROM centos:7
RUN yum update -y && yum install httpd -t
ENV TZ=Asia/Kolkata
EXPOSE 80
EXPOSE 443
CMD ["/usr/sbin/httpd","-D","FOREGROUND"]

