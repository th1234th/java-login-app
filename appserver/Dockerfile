FROM eclipse-temurin:8-jdk-jammy AS builder 

LABEL "Project"="web app demo Project"
LABEL "Author"="Thierno FALL"

RUN apt update && \
    apt install maven -y && \
    apt install git -y && \
    git clone https://thiernothedevops-admin@bitbucket.org/thiernothedevops/java-login-app.git && \
    cd java-login-app && \
    git checkout master && \
    mvn clean install 

FROM tomcat:8-jdk8-temurin-jammy
RUN rm -rf /usr/local/tomcat/webapps/*
COPY --from=builder java-login-app/target/webapp-1.0.war ROOT.war
RUN mv ROOT.war /usr/local/tomcat/webapps/

EXPOSE 8080
CMD ["catalina.sh", "run"]