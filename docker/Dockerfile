FROM openjdk:8u151-jdk-alpine3.7

ENV APP_HOME=/usr/src/app
WORKDIR $APP_HOME

COPY target/*.jar app.jar

EXPOSE 8070
ENTRYPOINT ["java","-jar","app.jar"]
