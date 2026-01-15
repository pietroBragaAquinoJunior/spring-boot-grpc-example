https://docs.spring.io/spring-grpc/reference/getting-started.html

grpcurl -d '{"name":"Hi"}' -plaintext localhost:8080 Simple.StreamHello

depois de criar o proto colocando o package certo,
./mvnw clean package
./mvnw spring-boot:run