FROM alpine:latest
MAINTAINER sam zzwangsh@163.com

# forward request and error logs to docker log collector
RUN apk --update add nginx
RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

EXPOSE 80

CMD [ "nginx","-g","daemon off;"]
