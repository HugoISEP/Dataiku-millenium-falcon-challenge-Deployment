FROM openjdk:20-jdk-slim
RUN addgroup --system spring && adduser --system spring --ingroup spring
USER spring:spring
COPY . .
EXPOSE 8080
ENTRYPOINT ["java","-jar", "-Dspring.profiles.active=prod", "/app.jar"]
