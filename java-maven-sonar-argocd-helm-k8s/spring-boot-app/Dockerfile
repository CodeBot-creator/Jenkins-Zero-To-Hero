# ✅ Use Java 17 base image (Alpine JRE)
FROM eclipse-temurin:17-jre-alpine

# Artifact path (built by Maven/Gradle)
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Run the app
ENTRYPOINT ["java", "-jar", "app.jar"]
