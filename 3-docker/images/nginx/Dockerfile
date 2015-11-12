FROM nginx

MAINTAINER Simon Constans "simon@constans.io"

# clean http directory
RUN rm -rf /usr/share/nginx/html/* && \
    rm -rf /etc/nginx/conf.d/*

ADD nginx-piwik.conf /etc/nginx/conf.d/nginx-piwik.conf

#RUN echo "upstream php-upstream { server php:9000; }" > /etc/nginx/conf.d/upstream.conf

EXPOSE 80
