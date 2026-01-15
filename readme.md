# Spring Boot gRPC Example

A simple and practical example of how to implement **gRPC** with **Spring Boot**, focusing on Protocol Buffers (protobuf) and service communication.

---

## ⚙️ Tech Stack
- Java 21  
- Spring Boot 3  
- Spring gRPC  
- Protocol Buffers (proto3)

---

## 🚀 Key Features
- **Protobuf Contract**: Definition of services in `.proto` files.
- **Auto-generation**: Automatic creation of Java stubs via Maven.
- **Streaming**: Example implementation of `Simple.StreamHello`.
- **Minimalist**: Clean code focused on gRPC core concepts.

---


### 1. Build and Generate Stubs

```bash
./mvnw clean package
```

### 2. Run the Application
```bash
./mvnw spring-boot:run
```

### 3. Test with gRPCurl
```bash
grpcurl -d '{"name":"Hi"}' -plaintext localhost:8080 Simple/StreamHello
```