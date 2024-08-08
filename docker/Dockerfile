####
# This Dockerfile is used in order to build a container that runs the Spring Boot application
####
FROM harbor-k8s.xsyxsc.cn/library/openjdk:8-jre-slim
COPY ./target/*.jar /app/target/spring-boot-docker.jar

EXPOSE 8080
ENTRYPOINT [ "java", "-jar", "/app/target/spring-boot-docker.jar", "--server.port=8080" ]