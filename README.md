# spring-boot-docker

1. To run jar from command line as SpringBoot without Docker enter the following command from within project level:
    ./mvnw package && java -jar target/spring-boot-docker-0.1.0.jar
    
2. To build as Docker container and cleanup afterwards enter the following commands:
    
    mvn clean install
    mvn dockerfile:build
    docker run -p 8080:8080 -t androiddavid/spring-boot-docker
    docker ps 
    docker stop <container id>
    docker rm <container id>
    docker container ls -a (if you want to see all containers)
    
    
    
    
