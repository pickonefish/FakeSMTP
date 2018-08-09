FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD fakeSMTP-*.jar app.jar
EXPOSE 25
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar", "--background", "--output-dir", "/output", "--port", "25", "--start-server"]
