FROM almalinux:8
RUN yum update -y
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
#this will not run when creator build the image
ONBUILD ADD index.html  /user/share/nginx/html/
ENTRYPOINT [ "nginx","-g","daemon off;" ]