FROM eclipse-temurin:17-jdk-alpine
LABEL authors="jacki"

VOLUME /tmp
ARG SRC_JAR=build/libs/*-SNAPSHOT.jar
ARG DEST_JAR=/configserver.jar

COPY ${SRC_JAR} ${DEST_JAR}

#ENTRYPOINT ["sh", "-c", "java ${JAVA_OPTS} -jar /${DEST_JAR} ${0} ${@}"]
#ENTRYPOINT ["sh", "-c", "java ${JAVA_OPTS} -jar /${DEST_JAR}"]

ENTRYPOINT ["java", "-jar", "/configserver.jar"]