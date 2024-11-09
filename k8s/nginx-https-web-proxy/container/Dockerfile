FROM openresty/openresty:1.25.3.2-1-alpine
RUN apk update \
    && apk upgrade \
    && apk add bash
COPY nginx.conf.template /etc/nginx/nginx.conf
COPY nginx_entrypoint.bash /
EXPOSE 443
ENTRYPOINT ["/nginx_entrypoint.bash"]
