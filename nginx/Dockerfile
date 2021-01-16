FROM nginx

LABEL name="nginx-for-testing" \
    version="1.0"

RUN apt-get update && apt-get install vim -y && apt-get clean all

COPY ./default.conf ./etc/nginx/conf.d/

EXPOSE 8080