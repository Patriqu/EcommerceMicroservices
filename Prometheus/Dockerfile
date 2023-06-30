FROM eclipse-temurin:17-jdk-alpine
LABEL authors="jacki"

VOLUME /tmp
ARG SRC_JAR=build/libs/*-SNAPSHOT.jar
ARG DEST_JAR=/prometheus.jar

COPY ${SRC_JAR} ${DEST_JAR}
#COPY src/main/resources/prometheus.yml prometheus-data/prometheus.yml

ENTRYPOINT ["java", "-jar", "/prometheus.jar"]