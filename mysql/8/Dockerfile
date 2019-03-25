ARG VERSION=latest
FROM mysql:${VERSION}

LABEL maintainer="Pierre-Louis Launay <laupi.frpar@gmail.com>"

COPY config/my.cnf /etc/mysql/conf.d/my.cnf

RUN chown -R mysql:root /var/lib/mysql/
