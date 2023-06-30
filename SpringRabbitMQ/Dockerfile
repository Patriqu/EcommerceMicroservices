FROM eclipse-temurin:17-jdk-alpine
LABEL authors="jacki"

VOLUME /tmp
ARG SRC_JAR=build/libs/*-SNAPSHOT.jar
ARG DEST_JAR=/spring-rabbitmq.jar

COPY ${SRC_JAR} ${DEST_JAR}

ENTRYPOINT ["java", "-jar", "${DEST_JAR}"]