FROM nginx:mainline-alpine

COPY ./scripts /

ENTRYPOINT ["/entrypoint.sh"]

RUN mkdir /etc/nginx/certs \
    && echo -e "\n\n\n\n\n\n\n" | openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/nginx/certs/nginx.key -out /etc/nginx/certs/nginx.crt

CMD ["nginx", "-g", "daemon off;"]
