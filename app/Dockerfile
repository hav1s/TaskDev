FROM nginx:alpine

COPY . /usr/share/nginx/html

COPY ./entrypoint.sh /

RUN chmod +x /entrypoint.sh

EXPOSE 80

#ENTRYPOINT ./entrypoint.sh
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]

CMD ["nginx", "-g", "daemon off;"]