FROM openjdk:8-jre
ADD build/libs/kotlin-webapi-1.0-SNAPSHOT.jar app.jar
ADD config/local.yml config.yml
EXPOSE 8080 8081
RUN apt-get update \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y \
    net-tools \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
ENTRYPOINT ["java","-jar", "app.jar", "server", "config.yml"]