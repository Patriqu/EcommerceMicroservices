FROM eclipse-temurin:17-jdk-alpine
LABEL authors="jacki"

VOLUME /tmp
ARG SRC_JAR=target/*-SNAPSHOT.jar
ARG DEST_JAR=/eureka-server.jar

COPY ${SRC_JAR} ${DEST_JAR}

ENTRYPOINT ["java", "-jar", "/eureka-server.jar"]