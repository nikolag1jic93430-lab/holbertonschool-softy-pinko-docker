FROM nginx:latest

COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/softy-pinko-front-end.conf

EXPOSE 9000

CMD ["nginx", "-g", "daemon off;"]
