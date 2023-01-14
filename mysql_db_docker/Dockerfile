FROM mysql:latest
ENV MYSQL_ROOT_PASSWORD password
ENV MYSQL_DATABASE tolldata
ADD CreateTable.sql /docker-entrypoint-initdb.d/
