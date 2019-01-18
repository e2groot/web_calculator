FROM openjdk:8-jre
ADD build/libs/kotlin-webapi-1.0-SNAPSHOT.jar app.jar
EXPOSE 8080 8081
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]