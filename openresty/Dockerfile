FROM openresty/openresty:alpine-fat as build

FROM openresty/openresty:alpine as release
COPY ./src /app

CMD ["/usr/local/openresty/bin/openresty", "-g", "daemon off;", "-p", "/app", "-c", "nginx.conf"]