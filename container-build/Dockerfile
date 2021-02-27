# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed -ie 's/^Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf &&\
    chgrp 0 -R /etc/httpd/logs


USER 1001


EXPOSE 8080
