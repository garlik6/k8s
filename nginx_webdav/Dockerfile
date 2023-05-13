FROM nginx:latest

COPY nginx_webdav.conf /etc/nginx/nginx.conf

RUN mkdir -p /var/www/webdav

RUN chown -R nginx:nginx /var/www/webdav && \
    chmod -R 770 /var/www/webdav

CMD ["nginx", "-g", "daemon off;"]
