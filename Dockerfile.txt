FROM eclipse-temurin:17
WORKDIR workspace
COPY target/demo-0.0.1-SNAPSHOT.jar demo.jar
COPY target/jacoco.exec jacoco.exec
ENTRYPOINT ["java", "-jar", "demo.jar"]
