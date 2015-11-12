FROM busybox

ENV PIWIK_VERSION 2.15.0

MAINTAINER Simon Constans "simon@constans.io"

# download piwik
RUN wget http://builds.piwik.org/piwik-${PIWIK_VERSION}.tar.gz && \
    tar -xzf piwik-${PIWIK_VERSION}.tar.gz && \
    rm piwik-${PIWIK_VERSION}.tar.gz && \
    chown -R www-data:www-data /piwik/ && \
    chmod -R 0755 /piwik/tmp

VOLUME /piwik
