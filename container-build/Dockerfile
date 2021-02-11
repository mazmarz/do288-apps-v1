# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed -i 's/Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf &&\  
  chmod g=u /var/log/httpd



EXPOSE 8080


