# Dependency Map

Spring PetClinic Microservices declares approximately 30 unique external dependencies across its 8 Maven modules, managed via Spring Boot 3.4.1 parent BOM and Spring Cloud 2024.0.0 BOM.

## Dependencies

```mermaid
flowchart LR
    App["spring-petclinic-microservices\nSpring Boot 3.4.1 / Java 17"]

    subgraph BOM["BOM / Parent"]
        SBParent["spring-boot-starter-parent v3.4.1"]
        SCDepsBOM["spring-cloud-dependencies v2024.0.0"]
        SpringAIBOM["spring-ai-bom v1.0.0-M4"]
    end

    subgraph Web["Web Frameworks"]
        SpringWeb["spring-boot-starter-web"]
        SCGateway["spring-cloud-starter-gateway"]
        SpringWebflux["spring-boot-starter-webflux"]
    end

    subgraph Cloud["Spring Cloud"]
        SCConfig["spring-cloud-starter-config"]
        SCEurekaClient["spring-cloud-starter-netflix-eureka-client"]
        SCEurekaServer["spring-cloud-starter-netflix-eureka-server"]
        SCConfigServer["spring-cloud-config-server"]
        SCCircuitBreaker["spring-cloud-starter-circuitbreaker-reactor-resilience4j"]
        Resilience4j["resilience4j-micrometer"]
    end

    subgraph DB["Database / ORM"]
        SpringDataJPA["spring-boot-starter-data-jpa"]
        HSQLDB["hsqldb (runtime)"]
        MySQLDriver["mysql-connector-j (runtime)"]
        DatasourceMicrometer["datasource-micrometer-spring-boot v1.0.2"]
        JaxbRuntime["jaxb-runtime"]
        JakartaXmlBind["jakarta.xml.bind-api"]
    end

    subgraph Cache["Caching"]
        SpringCache["spring-boot-starter-cache"]
        Caffeine["caffeine"]
        JCacheAPI["cache-api (javax.cache)"]
    end

    subgraph Observability["Observability"]
        Actuator["spring-boot-starter-actuator"]
        MicrometerPrometheus["micrometer-registry-prometheus"]
        MicrometerObs["micrometer-observation"]
        MicrometerTracing["micrometer-tracing-bridge-brave"]
        OtelZipkin["opentelemetry-exporter-zipkin"]
        ZipkinReporter["zipkin-reporter-brave"]
        Jolokia["jolokia-core v1.7.1"]
    end

    subgraph Admin["Management"]
        SBAdmin["spring-boot-admin-starter-server v3.4.1"]
        SBAdminUI["spring-boot-admin-server-ui v3.4.1"]
        ChaosMonkey["chaos-monkey-spring-boot v3.1.0"]
    end

    subgraph AI["AI / GenAI"]
        SpringAI["spring-ai-openai-spring-boot-starter v1.0.0-M4"]
    end

    subgraph Frontend["Frontend / WebJars"]
        AngularJS["angularjs v1.8.3"]
        Bootstrap["bootstrap v5.3.3"]
        FontAwesome["font-awesome"]
        AngularUIRouter["angular-ui-router"]
        Marked["marked"]
    end

    App -.->|"managed by"| BOM
    App -->|"web"| Web
    App -->|"cloud"| Cloud
    App -->|"persistence"| DB
    App -->|"caching"| Cache
    App -->|"observability"| Observability
    App -->|"management"| Admin
    App -->|"AI"| AI
    App -->|"frontend"| Frontend
    SBParent -.->|"governs"| Web
    SBParent -.->|"governs"| DB
    SCDepsBOM -.->|"governs"| Cloud
    SpringAIBOM -.->|"governs"| AI
```
