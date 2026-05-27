# spring-petclinic-microservices

## Summary

| Metric | Value |
|--------|-------|
| Total Issues | 21 |
| Mandatory Blockers | 6 |
| Potential Issues | 8 |

## Application Information

| Property | Value |
|----------|-------|
| Language | Java, Dockerfile |
| Frameworks | Spring Boot, Spring Cloud, Spring |
| Build tools | Maven |
| JDK version | 17 |

## Cloud Readiness Issues

| Issue Name | Criticality | Story Points | Occurrences |
|------------|-------------|--------------|-------------|
| Use of unsecured network protocols or URI libraries | Mandatory | 3 | [21](#Use_of_unsecured_network_protocols_or_URI_libraries) |
| Caching - Spring Boot Cache library | Mandatory | 5 | [9](#Caching_-_Spring_Boot_Cache_library) |
| File system - Java NIO | Mandatory | 3 | [4](#File_system_-_Java_NIO) |
| CRA: Hard-coded credentials in configuration files | Mandatory | 5 | [2](#CRA_Hard-coded_credentials_in_configuration_files) |
| File system - Java IO | Mandatory | 3 | [1](#File_system_-_Java_IO) |
| Embedded framework - Zipkin | Potential | 3 | [15](#Embedded_framework_-_Zipkin) |
| Embedded framework - Eureka Client | Potential | 2 | [7](#Embedded_framework_-_Eureka_Client) |
| Detects usage of Jakarta RESTful Web Services (JAX-RS) APIs | Potential | 5 | [7](#Detects_usage_of_Jakarta_RESTful_Web_Services_JAX-RS_APIs) |
| MySQL database found | Potential | 5 | [5](#MySQL_database_found) |
| Detects usage of Jakarta Persistence (JPA) APIs | Potential | 5 | [4](#Detects_usage_of_Jakarta_Persistence_JPA_APIs) |
| Restricted configurations found | Potential | 2 | [1](#Restricted_configurations_found) |
| Server port configuration found | Potential | 1 | [1](#Server_port_configuration_found) |
| Embedded framework - Eureka Server | Potential | 5 | [1](#Embedded_framework_-_Eureka_Server) |
| Avoid using hardcoded URLs (HTTP protocol) in source code | Optional | 3 | [23](#Avoid_using_hardcoded_URLs_HTTP_protocol_in_source_code) |
| Spring Cloud Config usage detected | Optional | 8 | [8](#Spring_Cloud_Config_usage_detected) |
| Localhost Usage | Optional | 3 | [1](#Localhost_Usage) |

### Issue Details

<details id="Use_of_unsecured_network_protocols_or_URI_libraries">
<summary><b>Use of unsecured network protocols or URI libraries</b> — affected files</summary>

- `docker/grafana/provisioning/datasources/all.yml (line 10)`
- `docker-compose.yml (line 10)`
- `docker-compose.yml (line 25)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 13)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/CustomersServiceClient.java (line 37)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java (line 34)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 5)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 50)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 13)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 20)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/AIDataProvider.java (line 27)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 67)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 9)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 45)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 16)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 13)`

</details>

<details id="Caching_-_Spring_Boot_Cache_library">
<summary><b>Caching - Spring Boot Cache library</b> — affected files</summary>

- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/src/main/java/org/springframework/samples/petclinic/vets/system/CacheConfig.java (line 18)`
- `spring-petclinic-vets-service/src/main/java/org/springframework/samples/petclinic/vets/web/VetResource.java (line 20)`

</details>

<details id="File_system_-_Java_NIO">
<summary><b>File system - Java NIO</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 27)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 26)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 24)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 25)`

</details>

<details id="CRA_Hard-coded_credentials_in_configuration_files">
<summary><b>CRA: Hard-coded credentials in configuration files</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/resources/application.yml (line 17)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 25)`

</details>

<details id="File_system_-_Java_IO">
<summary><b>File system - Java IO</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 22)`

</details>

<details id="Embedded_framework_-_Zipkin">
<summary><b>Embedded framework - Zipkin</b> — affected files</summary>

- `spring-petclinic-api-gateway/pom.xml (line 89)`
- `spring-petclinic-api-gateway/pom.xml (line 101)`
- `spring-petclinic-api-gateway/pom.xml (line 97)`
- `spring-petclinic-customers-service/pom.xml (line 90)`
- `spring-petclinic-customers-service/pom.xml (line 86)`
- `spring-petclinic-customers-service/pom.xml (line 78)`
- `spring-petclinic-vets-service/pom.xml (line 98)`
- `spring-petclinic-vets-service/pom.xml (line 106)`
- `spring-petclinic-vets-service/pom.xml (line 110)`
- `spring-petclinic-visits-service/pom.xml (line 89)`
- `spring-petclinic-visits-service/pom.xml (line 85)`
- `spring-petclinic-visits-service/pom.xml (line 77)`
- `spring-petclinic-genai-service/pom.xml (line 112)`
- `spring-petclinic-genai-service/pom.xml (line 124)`
- `spring-petclinic-genai-service/pom.xml (line 120)`

</details>

<details id="Embedded_framework_-_Eureka_Client">
<summary><b>Embedded framework - Eureka Client</b> — affected files</summary>

- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 58)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 68)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`

</details>

<details id="Detects_usage_of_Jakarta_RESTful_Web_Services_JAX-RS_APIs">
<summary><b>Detects usage of Jakarta RESTful Web Services (JAX-RS) APIs</b> — affected files</summary>

- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 68)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 58)`

</details>

<details id="MySQL_database_found">
<summary><b>MySQL database found</b> — affected files</summary>

- `spring-petclinic-customers-service/pom.xml (line 56)`
- `spring-petclinic-vets-service/pom.xml (line 85)`
- `spring-petclinic-visits-service/pom.xml (line 64)`
- `spring-petclinic-genai-service/pom.xml (line 99)`

</details>

<details id="Detects_usage_of_Jakarta_Persistence_JPA_APIs">
<summary><b>Detects usage of Jakarta Persistence (JPA) APIs</b> — affected files</summary>

- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-genai-service/pom.xml (line 49)`

</details>

<details id="Restricted_configurations_found">
<summary><b>Restricted configurations found</b> — affected files</summary>

- `spring-petclinic-config-server/src/main/resources/application.yml (line 1)`

</details>

<details id="Server_port_configuration_found">
<summary><b>Server port configuration found</b> — affected files</summary>

- `spring-petclinic-config-server/src/main/resources/application.yml (line 1)`

</details>

<details id="Embedded_framework_-_Eureka_Server">
<summary><b>Embedded framework - Eureka Server</b> — affected files</summary>

- `spring-petclinic-discovery-server/pom.xml (line 33)`

</details>

<details id="Avoid_using_hardcoded_URLs_HTTP_protocol_in_source_code">
<summary><b>Avoid using hardcoded URLs (HTTP protocol) in source code</b> — affected files</summary>

- `docker/grafana/provisioning/datasources/all.yml (line 10)`
- `docker-compose.yml (line 10)`
- `docker-compose.yml (line 25)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 13)`
- `spring-petclinic-config-server/src/main/resources/application.yml (line 7)`
- `spring-petclinic-config-server/src/test/resources/application.yml (line 6)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 67)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 9)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 45)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 13)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 20)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/AIDataProvider.java (line 27)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 16)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 5)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 50)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 13)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/CustomersServiceClient.java (line 37)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java (line 34)`

</details>

<details id="Spring_Cloud_Config_usage_detected">
<summary><b>Spring Cloud Config usage detected</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-visits-service/pom.xml (line 45)`
- `spring-petclinic-genai-service/pom.xml (line 64)`
- `spring-petclinic-discovery-server/pom.xml (line 37)`
- `spring-petclinic-api-gateway/pom.xml (line 63)`
- `spring-petclinic-admin-server/pom.xml (line 32)`
- `spring-petclinic-customers-service/pom.xml (line 46)`
- `spring-petclinic-vets-service/pom.xml (line 54)`

</details>

<details id="Localhost_Usage">
<summary><b>Localhost Usage</b> — affected files</summary>

- `docker/prometheus/prometheus.yml (line 12)`

</details>

## Upgrade Issues

| Issue Name | Criticality | Story Points | Occurrences |
|------------|-------------|--------------|-------------|
| Spring Boot Version Has Reached the End of OSS Support | Mandatory | 8 | [41](#Spring_Boot_Version_Has_Reached_the_End_of_OSS_Support) |
| Spring Framework Version is not the latest stable | Optional | 8 | [36](#Spring_Framework_Version_is_not_the_latest_stable) |
| Jakarta EE Version is not the latest stable | Optional | 8 | [10](#Jakarta_EE_Version_is_not_the_latest_stable) |
| Java Version is not the latest LTS | Optional | 8 | [1](#Java_Version_is_not_the_latest_LTS) |

### Issue Details

<details id="Spring_Boot_Version_Has_Reached_the_End_of_OSS_Support">
<summary><b>Spring Boot Version Has Reached the End of OSS Support</b> — affected files</summary>

- `spring-petclinic-vets-service/pom.xml (line 47)`
- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-vets-service/pom.xml (line 35)`
- `spring-petclinic-vets-service/pom.xml (line 26)`
- `spring-petclinic-vets-service/pom.xml (line 94)`
- `spring-petclinic-vets-service/pom.xml (line 30)`
- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 26)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-visits-service/pom.xml (line 38)`
- `spring-petclinic-visits-service/pom.xml (line 73)`
- `spring-petclinic-visits-service/pom.xml (line 34)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-genai-service/pom.xml (line 108)`
- `spring-petclinic-genai-service/pom.xml (line 27)`
- `spring-petclinic-genai-service/pom.xml (line 53)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-genai-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 41)`
- `spring-petclinic-genai-service/pom.xml (line 36)`
- `spring-petclinic-genai-service/pom.xml (line 32)`
- `spring-petclinic-genai-service/pom.xml (line 72)`
- `spring-petclinic-config-server/pom.xml (line 26)`
- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 26)`
- `spring-petclinic-api-gateway/pom.xml (line 44)`
- `spring-petclinic-api-gateway/pom.xml (line 34)`
- `spring-petclinic-api-gateway/pom.xml (line 71)`
- `spring-petclinic-api-gateway/pom.xml (line 52)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-api-gateway/pom.xml (line 39)`
- `spring-petclinic-admin-server/pom.xml (line 46)`
- `spring-petclinic-admin-server/pom.xml (line 28)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-customers-service/pom.xml (line 35)`
- `spring-petclinic-customers-service/pom.xml (line 74)`
- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-customers-service/pom.xml (line 27)`
- `spring-petclinic-customers-service/pom.xml (line 40)`

</details>

<details id="Spring_Framework_Version_is_not_the_latest_stable">
<summary><b>Spring Framework Version is not the latest stable</b> — affected files</summary>

- `spring-petclinic-customers-service/pom.xml (line 35)`
- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-customers-service/pom.xml (line 74)`
- `spring-petclinic-customers-service/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 94)`
- `spring-petclinic-vets-service/pom.xml (line 26)`
- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-vets-service/pom.xml (line 47)`
- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 34)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-visits-service/pom.xml (line 73)`
- `spring-petclinic-visits-service/pom.xml (line 38)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 108)`
- `spring-petclinic-genai-service/pom.xml (line 32)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-genai-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 72)`
- `spring-petclinic-genai-service/pom.xml (line 27)`
- `spring-petclinic-genai-service/pom.xml (line 53)`
- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-config-server/pom.xml (line 26)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 26)`
- `spring-petclinic-discovery-server/pom.xml (line 37)`
- `spring-petclinic-api-gateway/pom.xml (line 34)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-api-gateway/pom.xml (line 71)`
- `spring-petclinic-api-gateway/pom.xml (line 52)`
- `spring-petclinic-api-gateway/pom.xml (line 63)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-admin-server/pom.xml (line 28)`
- `spring-petclinic-admin-server/pom.xml (line 46)`
- `spring-petclinic-admin-server/pom.xml (line 32)`

</details>

<details id="Jakarta_EE_Version_is_not_the_latest_stable">
<summary><b>Jakarta EE Version is not the latest stable</b> — affected files</summary>

- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 27)`
- `spring-petclinic-genai-service/pom.xml (line 68)`
- `spring-petclinic-genai-service/pom.xml (line 78)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 58)`
- `spring-petclinic-vets-service/pom.xml (line 64)`

</details>

<details id="Java_Version_is_not_the_latest_LTS">
<summary><b>Java Version is not the latest LTS</b> — affected files</summary>

- `pom.xml (line 30)`

</details>

## Security Issues

> **Note:** These issues were generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

| Issue Name | Criticality | Story Points | Files |
|------------|-------------|--------------|-------|
| CWE-798: Use of Hard-coded Credentials | Optional | 5 | [1](#CWE-798_Use_of_Hard-coded_Credentials) |

### Security Issue Details

<details id="CWE-798_Use_of_Hard-coded_Credentials">
<summary><b>CWE-798: Use of Hard-coded Credentials</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/resources/application.yml:25`

</details>

---

## Codebase Insights

> **Note:** These documents are generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

> **Codebase Insights aren't available yet.**
>
> These documents are generated when assessment runs with **Full analysis** coverage. Re-run the assessment and set `analysisCoverage: full` to enable them.

[Share feedback](https://aka.ms/ghcp-appmod/feedback)
