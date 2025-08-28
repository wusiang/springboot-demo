#FROM openjdk:8-jre
#MAINTAINER CarpCap
#ADD target/app.jar /app.jar
#EXPOSE 9014
#ENTRYPOINT ["sh","-c","java  -jar $JAVA_OPTS  /app.jar"]
# 基于哪个镜像
FROM eclipse-temurin:21-jdk-alpine
ADD  target/app.jar /myapp/app.jar
ENTRYPOINT ["java","-XX:MetaspaceSize=256m","-Duser.timezone=GMT+8","-XX:MaxMetaspaceSize=256m","-Xms512m","-Xmx512m","-Xmn256m","-Xss256k","-Duser.timezone=GMT+8","-Djava.security.egd=file:/dev/./urandom","-jar","/myapp/app.jar"]
EXPOSE 9014