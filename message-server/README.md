# spring-boot-docker

If java is not intalled

choco install oracle17jdk

If maven is not intalle intal with choco

choco install maven

mvn clean package

java -jar target/message-server-0.0.1-SNAPSHOT.jar

open from localhost:8888/messages

expected mesage: Hello from Docker!

docker build --tag=message-server:latest .

docker run --name message-server -d -p 8887:8888 message-server

open from localhost:8887/messages


# Docker Compose

docker compose up -d

and ro stop and remove 

 docker compose down





