FROM adoptopenjdk/openjdk11-openj9:alpine-slim
EXPOSE 8080
ENV JAVA_OPTS="-Xms64m -Xmx128m -XX:MaxPermSize=128m"
COPY target/*.jar /deployment/application.jar

ENTRYPOINT java -jar $JAVA_OPTS /deployment/application.jar
