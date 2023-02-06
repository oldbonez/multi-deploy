FROM nginx:mainline-alpine
RUN apk update && apk upgrade && rm -vrf /var/cache/apk/*
COPY ./default.conf /etc/nginx/conf.d/default.conf
