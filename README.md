## Java Login App ##
Project based on [dptrealtime](https://bitbucket.org/dptrealtime/java-login-app/src/master/)

## We are using docker, maven, mysql, nginx and tomact
[Schema app](https://photos.app.goo.gl/cEuPgW5CoYcRBSQp8)

## How to create Table ##
## Below Query to create require TABLE schema to store Employee records ##
## You can create after the running container bd but the most efficient way is to create a init.sql script file 
## and copy it in docker-entrypoint-initdb.d/ 

CREATE TABLE Employee (
  id int unsigned auto_increment not null,
  first_name varchar(250),
  last_name varchar(250),
  email varchar(250),
  username varchar(250),
  password varchar(250),
  regdate timestamp,
  primary key (id)
);

