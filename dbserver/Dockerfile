FROM mysql:8.1

LABEL "Project"="Vprofile Project"
LABEL "Author"="Thierno FALL"

ENV MYSQL_ROOT_PASSWORD=dbpass
ENV MYSQL_DATABASE=demoDB

# Copy an SQL script to initialize the database
COPY init.sql /docker-entrypoint-initdb.d/


EXPOSE 3306