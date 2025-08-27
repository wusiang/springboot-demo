FROM openjdk:8-jre
MAINTAINER CarpCap
ADD target/app.jar /app.jar
EXPOSE 9014
ENTRYPOINT ["sh","-c","java  -jar $JAVA_OPTS  /app.jar"]