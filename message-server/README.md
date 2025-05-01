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

and to stop and remove 

docker compose down


# On AWS

If java no intalled, install:
```bash
sudo yum install java-17-amazon-corretto-devel
```

to remove run:

sudo yum remove java-17-amazon-corretto-devel


To install maven:
```bash
sudo yum install maven
```

```bash
git clone https://github.com/rsalgadoc/spring-boot-docker.git
```

NOTE:  
git pull is a convenient shortcut for completing both git fetch and git mergein the same command:


```bash
cd  spring-boot-docker
```

```bash
cd message-server/
```

```bash
mvn clean package
```

```bash
java -jar target/message-server-0.0.1-SNAPSHOT.jar
```

to test open a new terminal , add run:
```bash
curl localhost:8888/messages
```

# Docker Compose

```bash
docker compose up -d
```
and to stop and remove 

```bash
docker compose down
```

to test open
```bash
curl localhost:8887/messages
```

Spring Boot 2.3 added support for buildpacks. Put simply, instead of creating our own Dockerfile and building it using something like docker build, all we have to do is issue the following command:
```bash
mvn spring-boot:build-image
```

```bash
docker run -it -p9099:8888 message-server:0.0.1-SNAPSHOT
```

localhost:9099/messages