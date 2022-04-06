FROM adoptopenjdk:11-jre-hotspot
LABEL maintainer="Andrea 100"
LABEL version="0.0.1"
LABEL description="user rest api"
RUN apt update && apt install tzdata -y
ENV TZ="Europe/Rome"
RUN mkdir -p /opt/user/backend
COPY ../target/applicazioneProdottiRest-0.0.1-SNAPSHOT.jar /opt/user/backend
WORKDIR /opt/user/backend
ENTRYPOINT ["java", "-jar","applicazioneProdottiRest-0.0.1-SNAPSHOT.jar"]