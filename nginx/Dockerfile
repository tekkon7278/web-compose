FROM nginx

ARG APP_DOMAIN

RUN apt update

COPY ./files/conf.d/ /etc/nginx/conf.d/
RUN sed -i s/{%APP_DOMAIN%}/${APP_DOMAIN}/ /etc/nginx/conf.d/proxy.conf