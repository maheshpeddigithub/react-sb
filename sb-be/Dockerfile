# Create a new image for running the application
FROM openjdk:17-jdk

CMD ["./gradlew", "clean", "build"]
ARG JAR_FILE=./build/libs/sb-be-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} app.jar

# Expose the port on which the Spring Boot application will run
EXPOSE 8080

# Command to run the application
CMD ["java", "-jar", "app.jar"]