FROM nginx:1.25


LABEL "Project"="demo app"
LABEL "Author"="Thierno FALL"

RUN rm -rf /etc/nginx/conf.d/default.conf

COPY web-nginx.conf /etc/nginx/conf.d/nginx.conf
#COPY nginx.conf /etc/nginx/nginx.conf
EXPOSE 80
