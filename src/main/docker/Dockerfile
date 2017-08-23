FROM openjdk:8u111-jdk-alpine
MAINTAINER MarshallWu <wumanxing123@163.com>
ENV JAR_FILE_NAME @project.build.finalName@.jar
VOLUME /logs
ADD $JAR_FILE_NAME app.jar
EXPOSE 8080:8080
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar"]