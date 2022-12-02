FROM nginx:alpine

WORKDIR /app
COPY . .

RUN rm /etc/nginx/conf.d/default.conf
COPY --chown=nginx:nginx ./nginx.conf /etc/nginx/conf.d 

CMD ["nginx", "-g", "daemon off;"]