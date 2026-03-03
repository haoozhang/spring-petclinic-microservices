# Architecture Diagram

Spring PetClinic Microservices is a distributed application built on Spring Boot 3.4.1 and Spring Cloud 2024.0.0, consisting of eight services: five business microservices (API Gateway, Customers, Vets, Visits, GenAI), two infrastructure services (Config Server, Discovery Server), and one monitoring service (Admin Server).

## Application Architecture

```mermaid
flowchart TB
    Client["Browser Client\nAngularJS SPA"]

    subgraph Infrastructure["Infrastructure Services"]
        ConfigServer["Config Server\nSpring Cloud Config\nPort 8888"]
        DiscoveryServer["Discovery Server\nNetflix Eureka\nPort 8761"]
        AdminServer["Admin Server\nSpring Boot Admin\nPort 9090"]
    end

    subgraph Gateway["API Layer"]
        APIGateway["API Gateway\nSpring Cloud Gateway\nCircuit Breaker + Retry\nPort 8080"]
    end

    subgraph BusinessServices["Business Services"]
        CustomersService["Customers Service\nSpring Boot + JPA\nPort 8081"]
        VetsService["Vets Service\nSpring Boot + JPA\nCaffeine Cache\nPort 8083"]
        VisitsService["Visits Service\nSpring Boot + JPA\nPort 8082"]
        GenAIService["GenAI Service\nSpring AI OpenAI\nVector Store\nPort 8084"]
    end

    subgraph DataStores["Data Stores"]
        MySQL["MySQL Database"]
        HSQLDb["HSQLDB\nEmbedded Fallback"]
    end

    subgraph Observability["Observability"]
        Zipkin["Zipkin\nDistributed Tracing\nPort 9411"]
        Prometheus["Prometheus\nMetrics\nPort 9091"]
        Grafana["Grafana\nDashboards\nPort 3030"]
    end

    subgraph ExternalAPIs["External APIs"]
        OpenAI["OpenAI API\nor Azure OpenAI"]
    end

    Client -->|HTTP| APIGateway
    APIGateway -->|lb://customers-service| CustomersService
    APIGateway -->|lb://vets-service| VetsService
    APIGateway -->|lb://visits-service| VisitsService
    APIGateway -->|lb://genai-service| GenAIService

    GenAIService -->|WebClient REST| CustomersService

    ConfigServer -->|provides config| APIGateway
    ConfigServer -->|provides config| CustomersService
    ConfigServer -->|provides config| VetsService
    ConfigServer -->|provides config| VisitsService
    ConfigServer -->|provides config| GenAIService
    ConfigServer -->|provides config| AdminServer

    DiscoveryServer -->|service registry| APIGateway
    DiscoveryServer -->|service registry| CustomersService
    DiscoveryServer -->|service registry| VetsService
    DiscoveryServer -->|service registry| VisitsService
    DiscoveryServer -->|service registry| GenAIService
    DiscoveryServer -->|service registry| AdminServer

    CustomersService -->|JPA| MySQL
    VetsService -->|JPA| MySQL
    VisitsService -->|JPA| MySQL
    GenAIService -->|JPA| MySQL
    CustomersService -.->|fallback| HSQLDb
    VetsService -.->|fallback| HSQLDb
    VisitsService -.->|fallback| HSQLDb

    GenAIService -->|API calls| OpenAI

    CustomersService -->|traces| Zipkin
    VetsService -->|traces| Zipkin
    VisitsService -->|traces| Zipkin
    GenAIService -->|traces| Zipkin
    APIGateway -->|traces| Zipkin

    CustomersService -->|metrics| Prometheus
    VetsService -->|metrics| Prometheus
    VisitsService -->|metrics| Prometheus
    GenAIService -->|metrics| Prometheus
    APIGateway -->|metrics| Prometheus
    Prometheus -->|data source| Grafana

    AdminServer -->|monitors via Eureka| DiscoveryServer
```
