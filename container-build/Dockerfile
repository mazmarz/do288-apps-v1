# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed -ie 's/^Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf &&\
    chgrp 0 -R /var/log/httpd &&\
    chmod -R g=u /var/log/httpd /var/run/httpd


USER 1001


EXPOSE 8080
