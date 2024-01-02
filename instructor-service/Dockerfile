# Stage 1: Build the application
#FROM gradle:8.4-jdk17-alpine as builder
#WORKDIR /app
#COPY . .
#RUN gradle build
#
## Stage 2: Create the final image
#FROM openjdk:17
#WORKDIR /app
### Copy the jar file from the build/libs directory to the Docker image
#COPY --from=builder /app/build/libs/*-SNAPSHOT.jar student-service-app.jar
#ENTRYPOINT ["java", "-jar", "/app/student-service-app.jar"]
#EXPOSE 8086


FROM openjdk:17
WORKDIR /app
COPY . .
ENTRYPOINT ["java", "-jar", "/app/DEVKH-INSTRUCTOR-SERVICE-0.0.1-SNAPSHOT.jar"]
EXPOSE 8081
