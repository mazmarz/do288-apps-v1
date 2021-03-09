# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed  -ie 's/^Listen 8080/Listen 80/' /etc/httpd/conf/httpd.conf 
