# Architecture Diagram

Spring PetClinic Microservices is a Spring Boot 3.4.1 application composed of independent services coordinated by Spring Cloud components for service discovery, centralized configuration, and an API gateway.

## Application Architecture

```mermaid
flowchart TD
    subgraph Client["Client Layer"]
        Browser["Web Browser"]
    end
    subgraph Gateway["API Gateway - Spring Cloud Gateway :8080"]
        GW["api-gateway"]
    end
    subgraph Infra["Infrastructure Services"]
        Config["config-server\nSpring Cloud Config :8888"]
        Discovery["discovery-server\nEureka :8761"]
        Admin["admin-server\nSpring Boot Admin :9090"]
        Tracing["tracing-server\nZipkin :9411"]
        Grafana["grafana-server :3030"]
        Prometheus["prometheus-server :9091"]
    end
    subgraph Business["Business Microservices - Spring Boot 3.4.1"]
        Customers["customers-service :8081"]
        Visits["visits-service :8082"]
        Vets["vets-service :8083"]
        GenAI["genai-service :8084"]
    end
    subgraph Data["Data Layer"]
        HSQLDB1[("HSQLDB\ncustomers")]
        HSQLDB2[("HSQLDB\nvisits")]
        HSQLDB3[("HSQLDB\nvets")]
        Cache[("Spring Cache\nvets")]
    end
    subgraph External["External Services"]
        OpenAI["OpenAI / Azure OpenAI\ngpt-4o"]
    end

    Browser -->|"HTTP :8080"| GW
    GW -->|"routes"| Customers
    GW -->|"routes"| Visits
    GW -->|"routes"| Vets
    GW -->|"routes"| GenAI
    Config -->|"provides config"| GW
    Config -->|"provides config"| Customers
    Config -->|"provides config"| Visits
    Config -->|"provides config"| Vets
    Config -->|"provides config"| GenAI
    Discovery -->|"registers"| GW
    Discovery -->|"registers"| Customers
    Discovery -->|"registers"| Visits
    Discovery -->|"registers"| Vets
    Discovery -->|"registers"| GenAI
    Customers -->|"JPA / HSQLDB"| HSQLDB1
    Visits -->|"JPA / HSQLDB"| HSQLDB2
    Vets -->|"JPA / HSQLDB"| HSQLDB3
    Vets -->|"cached"| Cache
    GenAI -->|"chat completions"| OpenAI
    Prometheus -->|"scrapes metrics"| Business
    Grafana -->|"queries"| Prometheus
    Admin -->|"monitors"| Business
    Business -->|"traces"| Tracing
```

## Component Relationships

```mermaid
flowchart LR
    subgraph Presentation["Presentation"]
        GWCtrl["ApiGatewayController"]
        FallCtrl["FallbackController"]
        OwnerRes["OwnerResource"]
        PetRes["PetResource"]
        VetRes["VetResource"]
        VisitRes["VisitResource"]
        VectorCtrl["VectorStoreController"]
    end
    subgraph Business["Business Logic"]
        CustomersClient["CustomersServiceClient"]
        VisitsClient["VisitsServiceClient"]
        PetclinicChat["PetclinicChatClient"]
        AIDataProv["AIDataProvider"]
        AIFuncConf["AIFunctionConfiguration"]
    end
    subgraph DataAccess["Data Access"]
        OwnerRepo["OwnerRepository"]
        PetRepo["PetRepository"]
        VetRepo["VetRepository"]
        VisitRepo["VisitRepository"]
    end
    subgraph Infra["Infrastructure"]
        CacheConf["CacheConfig"]
        MetricConf["MetricConfig"]
        MapperSvc["OwnerEntityMapper"]
    end

    GWCtrl -->|"delegates"| CustomersClient
    GWCtrl -->|"delegates"| VisitsClient
    OwnerRes -->|"queries"| OwnerRepo
    PetRes -->|"queries"| PetRepo
    VetRes -->|"queries"| VetRepo
    VisitRes -->|"queries"| VisitRepo
    VectorCtrl -->|"delegates"| AIDataProv
    PetclinicChat -->|"uses"| AIFuncConf
    AIFuncConf -->|"invokes"| AIDataProv
    OwnerRes -->|"maps"| MapperSvc
    VetRepo -.->|"cached by"| CacheConf
    VetRes -.->|"metrics"| MetricConf
    VisitRes -.->|"metrics"| MetricConf
```
