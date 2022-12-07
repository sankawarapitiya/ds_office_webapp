#FROM openjdk:17
#LABEL maintainer="attom.com"
#ADD target/api-gateway-0.0.1.jar spring-microservice-api-gateway.jar
##EXPOSE ${SERVER_PORT}
#EXPOSE 8080
#ENTRYPOINT ["java", "-jar", "spring-microservice-api-gateway.jar"]

FROM openjdk:17
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} cloud-gateway.jar
ENTRYPOINT ["java","-jar","/cloud-gateway.jar"]
EXPOSE 9191