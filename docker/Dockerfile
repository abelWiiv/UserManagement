## Build stage
#FROM maven:3.8.6-openjdk-17 AS build
#WORKDIR /app
#COPY pom.xml .
#RUN mvn dependency:go-offline
#COPY src ./src
#RUN mvn package -DskipTests
#
## Run stage
#FROM openjdk:17-jdk-slim
#WORKDIR /app
#COPY --from=build /app/target/user-management-service-*.jar app.jar
#EXPOSE 8081
#ENTRYPOINT ["java", "-jar", "app.jar"]