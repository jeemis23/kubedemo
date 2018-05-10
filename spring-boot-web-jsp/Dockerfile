FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD target/*.jar TestApplication-0.0.1-SNAPSHOT.jar

ENV JAVA_OPTS=""
ENV SPRING_PROFILE="default"

ENTRYPOINT exec java $JAVA_OPTS \
 -Dspring.profiles.active=$SPRING_PROFILE \
 -jar TestApplication-0.0.1-SNAPSHOT.jar
