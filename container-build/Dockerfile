# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed -i 's/Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf &&\  
  chmod g=u /var/log/httpd

USER 1001

EXPOSE 8080

CMD /usr/sbin/httpd -DFOREGROUND

