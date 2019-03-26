ARG VERSION=latest
FROM mysql:${VERSION}

LABEL maintainer="Pierre-Louis Launay <laupi.frpar@gmail.com>"

ARG VERSION_CONFIG=8
COPY /config/${VERSION_CONFIG}/my.cnf /etc/mysql/conf.d/my.cnf

RUN chown -R mysql:root /var/lib/mysql/
