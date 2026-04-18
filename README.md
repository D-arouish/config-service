# config-service

Spring Cloud Config Server for the e-commerce microservices ecosystem. This service centralizes externalized configuration and serves it to the other services at startup.

## Responsibilities

- exposes a central configuration server
- registers with Eureka for service discovery
- pulls configuration from `D-arouish/ecom-app-config-repo`
- exposes actuator endpoints for health and monitoring

## Stack

- Java 17
- Spring Boot
- Spring Cloud Config Server
- Eureka Client
- Spring Boot Actuator

## Default Configuration

- Port: `9999`
- Discovery URL: `DISCOVERY_SERVICE_URL`, defaulting to `http://localhost:8761/eureka`

## Run Locally

```bash
./mvnw spring-boot:run
```

Start `discovery-service` first when running the full platform.
