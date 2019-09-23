FROM openjdk:8-jdk-alpine
ENV APP_FILE TestEureka-0.0.1-SNAPSHOT.jar
VOLUME /tmp

# Add Spring Boot TestEureka-0.0.1-SNAPSHOT.jar to Container
COPY target/$APP_FILE .

ENV JAVA_OPTS=""

# Fire up our Spring Boot springdemo by default
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Dspring.profiles.active=dev -jar /$APP_FILE" ]