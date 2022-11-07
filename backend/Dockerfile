FROM openjdk:20-jdk-slim
RUN addgroup --system spring && adduser --system spring --ingroup spring
USER spring:spring
ARG JAR_FILE=*.jar
COPY ${JAR_FILE} app.jar
COPY millennium-falcon.json  millennium-falcon.json
COPY universe.db  universe.db
EXPOSE 8080
ENTRYPOINT ["java","-jar", "-Dspring.profiles.active=prod", "/app.jar"]
