# NotificationService - Spring Boot Microservice

## Requirements

To run this project, you will need to have the following installed on your system:

- Java (version 17)

- Spring Boot (version 3.0.6)

- Maven (version 3.9.1)


# Running locally with maven
```
mvn install
```
```
mvn spring-boot:run
```

# Running with docker
To help ensure consistently correct startup across multiple platforms, you may choose to use Docker to containerize your application.  Installation steps for docker can be found on their main page.
https://docs.docker.com/engine/install/

With Docker installed, you can build your a new image. This build needs to be run after any changes are made to the source code.
```
docker build -t notification-service . 
```

After the image builds successfully, run a container from that image.
```
docker run -p 8080:8080 notification-service:latest
```

When you are done testing, stop the server and remove the container.
```
docker rm -f notification-service
```

# Running with docker-compose
docker-compose up
