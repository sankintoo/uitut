FROM adoptopenjdk/openjdk11:ubi
RUN mkdir /opt/app
ARG JAR_FILE=target/idp-microservice-0.0.1-SNAPSHOT.jar
WORKDIR /opt/app
COPY ${JAR_FILE} /opt/app/idpApp.jar
CMD ["java", "-jar", "/opt/app/idpApp.jar"]


#FROM openjdk:8-jdk-alpine
#ARG JAR_FILE=target/*.jar
#COPY ${JAR_FILE} app.jar
#ENTRYPOINT ["java","-jar","/app.jar"]