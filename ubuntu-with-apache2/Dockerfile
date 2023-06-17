FROM ubuntu
RUN apt update
RUN apt install apache2 -y
RUN apt install apache2-utils -y
ENV TZ=Asia/Kolkata
RUN apt clean
EXPOSE 80
EXPOSE 443
CMD ["apache2ctl", "-D","FOREGROUND"]

