# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent


LABEL io.openshift.expose-services="8080:http"

ENV DIRS /var/log/httpd /run/httpd

RUN sed  -ie 's/^Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf &&\
  chgrp 0 ${DIRS} && chmod g=u ${DIRS}

EXPOSE 8080
USER 1001
