# Option 1 with openjdk:17-jdk-alpine 
#FROM openjdk:17-jdk-alpine
#COPY target/message-server-0.0.1-SNAPSHOT.jar message-server-0.0.1-SNAPSHOT.jar
#ENTRYPOINT ["java","-jar","/message-server-0.0.1-SNAPSHOT.jar"]


# Option 2 with amazoncorretto:17-alpine-jdk
FROM amazoncorretto:17-alpine-jdk
COPY target/message-server-0.0.1-SNAPSHOT.jar message-server-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java","-jar","/message-server-0.0.1-SNAPSHOT.jar"]


