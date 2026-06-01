# spring-petclinic-microservices

## Summary

| Metric | Value |
|--------|-------|
| Total Issues | 96 |
| Mandatory Blockers | 49 |
| Potential Issues | 12 |

## Component Information

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
| Embedded framework - Eureka Server | Potential | 5 | [1](#Embedded_framework_-_Eureka_Server) |
| Server port configuration found | Potential | 1 | [1](#Server_port_configuration_found) |
| Restricted configurations found | Potential | 2 | [1](#Restricted_configurations_found) |
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
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 9)`
- `spring-petclinic-genai-service/src/main/resources/application.yml (line 45)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-customers-service/src/main/resources/application.yml (line 13)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-vets-service/src/main/resources/application.yml (line 16)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/AIDataProvider.java (line 27)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 5)`
- `spring-petclinic-visits-service/src/main/resources/application.yml (line 13)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 67)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-discovery-server/src/main/resources/application.yml (line 20)`

</details>

<details id="Caching_-_Spring_Boot_Cache_library">
<summary><b>Caching - Spring Boot Cache library</b> — affected files</summary>

- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-vets-service/src/main/java/org/springframework/samples/petclinic/vets/system/CacheConfig.java (line 18)`
- `spring-petclinic-vets-service/src/main/java/org/springframework/samples/petclinic/vets/web/VetResource.java (line 20)`

</details>

<details id="File_system_-_Java_NIO">
<summary><b>File system - Java NIO</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 26)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 27)`
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

- `spring-petclinic-customers-service/pom.xml (line 86)`
- `spring-petclinic-customers-service/pom.xml (line 90)`
- `spring-petclinic-customers-service/pom.xml (line 78)`
- `spring-petclinic-vets-service/pom.xml (line 106)`
- `spring-petclinic-vets-service/pom.xml (line 98)`
- `spring-petclinic-vets-service/pom.xml (line 110)`
- `spring-petclinic-visits-service/pom.xml (line 85)`
- `spring-petclinic-visits-service/pom.xml (line 77)`
- `spring-petclinic-visits-service/pom.xml (line 89)`
- `spring-petclinic-genai-service/pom.xml (line 120)`
- `spring-petclinic-genai-service/pom.xml (line 124)`
- `spring-petclinic-genai-service/pom.xml (line 112)`
- `spring-petclinic-api-gateway/pom.xml (line 101)`
- `spring-petclinic-api-gateway/pom.xml (line 97)`
- `spring-petclinic-api-gateway/pom.xml (line 89)`

</details>

<details id="Embedded_framework_-_Eureka_Client">
<summary><b>Embedded framework - Eureka Client</b> — affected files</summary>

- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 58)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 68)`

</details>

<details id="Detects_usage_of_Jakarta_RESTful_Web_Services_JAX-RS_APIs">
<summary><b>Detects usage of Jakarta RESTful Web Services (JAX-RS) APIs</b> — affected files</summary>

- `spring-petclinic-vets-service/pom.xml (line 58)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 68)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`

</details>

<details id="MySQL_database_found">
<summary><b>MySQL database found</b> — affected files</summary>

- `spring-petclinic-genai-service/pom.xml (line 99)`
- `spring-petclinic-customers-service/pom.xml (line 56)`
- `spring-petclinic-vets-service/pom.xml (line 85)`
- `spring-petclinic-visits-service/pom.xml (line 64)`

</details>

<details id="Detects_usage_of_Jakarta_Persistence_JPA_APIs">
<summary><b>Detects usage of Jakarta Persistence (JPA) APIs</b> — affected files</summary>

- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-genai-service/pom.xml (line 49)`

</details>

<details id="Embedded_framework_-_Eureka_Server">
<summary><b>Embedded framework - Eureka Server</b> — affected files</summary>

- `spring-petclinic-discovery-server/pom.xml (line 33)`

</details>

<details id="Server_port_configuration_found">
<summary><b>Server port configuration found</b> — affected files</summary>

- `spring-petclinic-config-server/src/main/resources/application.yml (line 1)`

</details>

<details id="Restricted_configurations_found">
<summary><b>Restricted configurations found</b> — affected files</summary>

- `spring-petclinic-config-server/src/main/resources/application.yml (line 1)`

</details>

<details id="Avoid_using_hardcoded_URLs_HTTP_protocol_in_source_code">
<summary><b>Avoid using hardcoded URLs (HTTP protocol) in source code</b> — affected files</summary>

- `docker/grafana/provisioning/datasources/all.yml (line 10)`
- `docker-compose.yml (line 10)`
- `docker-compose.yml (line 25)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 5)`
- `spring-petclinic-admin-server/src/main/resources/application.yml (line 13)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/CustomersServiceClient.java (line 37)`
- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java (line 34)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 5)`
- `spring-petclinic-api-gateway/src/main/resources/application.yml (line 50)`
- `spring-petclinic-config-server/src/main/resources/application.yml (line 7)`
- `spring-petclinic-config-server/src/test/resources/application.yml (line 6)`
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

<details id="Spring_Cloud_Config_usage_detected">
<summary><b>Spring Cloud Config usage detected</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 37)`
- `spring-petclinic-api-gateway/pom.xml (line 63)`
- `spring-petclinic-admin-server/pom.xml (line 32)`
- `spring-petclinic-customers-service/pom.xml (line 46)`
- `spring-petclinic-vets-service/pom.xml (line 54)`
- `spring-petclinic-visits-service/pom.xml (line 45)`
- `spring-petclinic-genai-service/pom.xml (line 64)`

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

- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-vets-service/pom.xml (line 47)`
- `spring-petclinic-vets-service/pom.xml (line 35)`
- `spring-petclinic-vets-service/pom.xml (line 26)`
- `spring-petclinic-vets-service/pom.xml (line 94)`
- `spring-petclinic-vets-service/pom.xml (line 30)`
- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 38)`
- `spring-petclinic-visits-service/pom.xml (line 73)`
- `spring-petclinic-visits-service/pom.xml (line 26)`
- `spring-petclinic-visits-service/pom.xml (line 34)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-genai-service/pom.xml (line 32)`
- `spring-petclinic-genai-service/pom.xml (line 53)`
- `spring-petclinic-genai-service/pom.xml (line 36)`
- `spring-petclinic-genai-service/pom.xml (line 41)`
- `spring-petclinic-genai-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 27)`
- `spring-petclinic-genai-service/pom.xml (line 108)`
- `spring-petclinic-genai-service/pom.xml (line 72)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-config-server/pom.xml (line 26)`
- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 26)`
- `spring-petclinic-api-gateway/pom.xml (line 71)`
- `spring-petclinic-api-gateway/pom.xml (line 52)`
- `spring-petclinic-api-gateway/pom.xml (line 44)`
- `spring-petclinic-api-gateway/pom.xml (line 34)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-api-gateway/pom.xml (line 39)`
- `spring-petclinic-admin-server/pom.xml (line 28)`
- `spring-petclinic-admin-server/pom.xml (line 46)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 74)`
- `spring-petclinic-customers-service/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 27)`
- `spring-petclinic-customers-service/pom.xml (line 35)`
- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-customers-service/pom.xml (line 50)`

</details>

<details id="Spring_Framework_Version_is_not_the_latest_stable">
<summary><b>Spring Framework Version is not the latest stable</b> — affected files</summary>

- `spring-petclinic-genai-service/pom.xml (line 32)`
- `spring-petclinic-genai-service/pom.xml (line 27)`
- `spring-petclinic-genai-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 45)`
- `spring-petclinic-genai-service/pom.xml (line 53)`
- `spring-petclinic-genai-service/pom.xml (line 108)`
- `spring-petclinic-genai-service/pom.xml (line 72)`
- `spring-petclinic-config-server/pom.xml (line 26)`
- `spring-petclinic-config-server/pom.xml (line 33)`
- `spring-petclinic-discovery-server/pom.xml (line 37)`
- `spring-petclinic-discovery-server/pom.xml (line 26)`
- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 71)`
- `spring-petclinic-api-gateway/pom.xml (line 63)`
- `spring-petclinic-api-gateway/pom.xml (line 52)`
- `spring-petclinic-api-gateway/pom.xml (line 34)`
- `spring-petclinic-api-gateway/pom.xml (line 48)`
- `spring-petclinic-admin-server/pom.xml (line 40)`
- `spring-petclinic-admin-server/pom.xml (line 46)`
- `spring-petclinic-admin-server/pom.xml (line 28)`
- `spring-petclinic-admin-server/pom.xml (line 32)`
- `spring-petclinic-customers-service/pom.xml (line 74)`
- `spring-petclinic-customers-service/pom.xml (line 40)`
- `spring-petclinic-customers-service/pom.xml (line 31)`
- `spring-petclinic-customers-service/pom.xml (line 35)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 47)`
- `spring-petclinic-vets-service/pom.xml (line 43)`
- `spring-petclinic-vets-service/pom.xml (line 94)`
- `spring-petclinic-vets-service/pom.xml (line 26)`
- `spring-petclinic-vets-service/pom.xml (line 39)`
- `spring-petclinic-visits-service/pom.xml (line 34)`
- `spring-petclinic-visits-service/pom.xml (line 30)`
- `spring-petclinic-visits-service/pom.xml (line 73)`
- `spring-petclinic-visits-service/pom.xml (line 38)`
- `spring-petclinic-visits-service/pom.xml (line 49)`

</details>

<details id="Jakarta_EE_Version_is_not_the_latest_stable">
<summary><b>Jakarta EE Version is not the latest stable</b> — affected files</summary>

- `spring-petclinic-discovery-server/pom.xml (line 33)`
- `spring-petclinic-api-gateway/pom.xml (line 67)`
- `spring-petclinic-admin-server/pom.xml (line 36)`
- `spring-petclinic-customers-service/pom.xml (line 50)`
- `spring-petclinic-vets-service/pom.xml (line 64)`
- `spring-petclinic-vets-service/pom.xml (line 58)`
- `spring-petclinic-visits-service/pom.xml (line 49)`
- `spring-petclinic-genai-service/pom.xml (line 68)`
- `spring-petclinic-genai-service/pom.xml (line 78)`
- `spring-petclinic-genai-service/pom.xml (line 27)`

</details>

<details id="Java_Version_is_not_the_latest_LTS">
<summary><b>Java Version is not the latest LTS</b> — affected files</summary>

- `pom.xml (line 30)`

</details>

## Security Issues

> **Note:** These issues were generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

| Issue Name | Criticality | Story Points | Files |
|------------|-------------|--------------|-------|
| CVE-2026-43512: Apache Tomcat - Digest authenticator will authenticate any unknown user | Mandatory | 1 | 0 |
| CVE-2026-43515: Apache Tomcat - Security constraints not correctly applied | Mandatory | 1 | 0 |
| CVE-2026-41293: Apache Tomcat - HTTP/2 request headers not validated | Mandatory | 1 | 0 |
| CVE-2025-24813: Apache Tomcat: Potential RCE and/or information disclosure and/or information corruption with partial PUT | Mandatory | 1 | 0 |
| CVE-2025-12383: Eclipse Jersey has a Race Condition | Mandatory | 1 | 0 |
| CVE-2026-40982: Spring Cloud Config vulnerable to Path Traversal | Mandatory | 1 | [1](#CVE-2026-40982_Spring_Cloud_Config_vulnerable_to_Path_Traversal) |
| CVE-2026-41901: Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns | Mandatory | 1 | 0 |
| CVE-2026-40478: Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf | Mandatory | 1 | 0 |
| CVE-2026-40477: Improper restriction of the scope of accessible objects in Thymeleaf expressions | Mandatory | 1 | 0 |
| CVE-2024-47072: XStream is vulnerable to a Denial of Service attack due to stack overflow from a manipulated binary input stream | Mandatory | 1 | 0 |
| CVE-2026-42587: Netty: HttpContentDecompressor maxAllocation bypass when Content-Encoding set to br/zstd/snappy leads to decompression bomb DoS | Mandatory | 1 | 0 |
| CVE-2026-42584: Netty has HttpClientCodec response desynchronization | Mandatory | 1 | 0 |
| CVE-2026-42583: Netty Lz4FrameDecoder is vulnerable to resource exhaustion  | Mandatory | 1 | 0 |
| CVE-2026-42579: Netty has a DNS Codec Input Validation Bypass (Encoder + Decoder) | Mandatory | 1 | 0 |
| CVE-2026-33871: Netty HTTP/2 CONTINUATION Frame Flood DoS via Zero-Byte Frame Bypass | Mandatory | 1 | 0 |
| CVE-2026-33870: Netty: HTTP Request Smuggling via Chunked Extension Quoted-String Parsing | Mandatory | 1 | 0 |
| CVE-2025-55163: Netty affected by MadeYouReset HTTP/2 DDoS vulnerability | Mandatory | 1 | 0 |
| CVE-2025-24970: SslHandler doesn't correctly validate packets which can lead to native crash when using native SSLEngine | Mandatory | 1 | 0 |
| CVE-2026-41284: Apache Tomcat: Unbounded read in WebDAV LOCK and  PROPFIND handling | Mandatory | 1 | 0 |
| CVE-2026-43513: Apache Tomcat: LockOutRealm treats user names as case-sensitive | Mandatory | 1 | 0 |
| CVE-2026-42498: Apache Tomcat - WebSocket authentication header exposure | Mandatory | 1 | 0 |
| CVE-2026-5598: Bouncy Castle Has Covert Timing Channel Vulnerability | Mandatory | 1 | 0 |
| CVE-2026-34483: Apache Tomcat has an Improper Encoding or Escaping of Output vulnerability in the JsonAccessLogValve | Mandatory | 1 | 0 |
| CVE-2026-34487: Apache Tomcat vulnerable to Insertion of Sensitive Information into Log File | Mandatory | 1 | 0 |
| CVE-2026-24880: Apache Tomcat has an HTTP Request/Response Smuggling vulnerability | Mandatory | 1 | 0 |
| CVE-2026-24734: Apache Tomcat has an Improper Input Validation vulnerability | Mandatory | 1 | 0 |
| CVE-2025-55752: Apache Tomcat Vulnerable to Relative Path Traversal | Mandatory | 1 | 0 |
| CVE-2025-48989: Apache Tomcat Improper Resource Shutdown or Release vulnerability | Mandatory | 1 | 0 |
| CVE-2025-53506: Apache Tomcat Coyote vulnerable to Denial of Service via excessive HTTP/2 streams | Mandatory | 1 | 0 |
| CVE-2025-52520: Apache Tomcat Catalina is vulnerable to DoS attack through bypassing of size limits | Mandatory | 1 | 0 |
| CVE-2025-48988: Apache Tomcat - DoS in multipart upload | Mandatory | 1 | 0 |
| CVE-2025-27820: Apache HttpClient disables domain checks | Mandatory | 1 | 0 |
| CVE-2026-40972: Spring Boot DevTools remote secret comparison is vulnerable to timing attacks | Mandatory | 1 | [1](#CVE-2026-40972_Spring_Boot_DevTools_remote_secret_comparison_is_vulnerable_to_timing_attacks) |
| CVE-2026-22733: Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints | Mandatory | 1 | [5](#CVE-2026-22733_Spring_Boot_has_an_Authentication_Bypass_under_Actuator_CloudFoundry_endpoints) |
| CVE-2026-22731: Spring Boot has an Authentication Bypass under Actuator Health groups paths | Mandatory | 1 | [5](#CVE-2026-22731_Spring_Boot_has_an_Authentication_Bypass_under_Actuator_Health_groups_paths) |
| CVE-2026-41002: Spring Cloud Config Server Susceptible To TOCTOU Attack | Mandatory | 1 | [1](#CVE-2026-41002_Spring_Cloud_Config_Server_Susceptible_To_TOCTOU_Attack) |
| CVE-2026-40973: Spring Boot accepts predictable temp directory without ownership verification | Mandatory | 1 | 0 |
| CVE-2026-22739: Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access | Mandatory | 1 | [1](#CVE-2026-22739_Spring_Cloud_Config_Server_Path_Traversal_via_Profile_Parameter_Allows_Arbitrary_File_Access) |
| CVE-2025-41253: Spring Cloud Gateway Server Webflux is vulnerable to Expression Language Injection | Mandatory | 1 | 0 |
| CVE-2025-41249: Spring Framework annotation detection mechanism may result in improper authorization | Mandatory | 1 | 0 |
| CVE-2025-41235: Spring Cloud Gateway Server Forwards Headers from Untrusted Proxies | Mandatory | 1 | 0 |
| CVE-2025-22235: Spring Boot EndpointRequest.to() creates wrong matcher if actuator endpoint is not exposed | Mandatory | 1 | 0 |
| CVE-2025-22228: Spring Security Does Not Enforce Password Length | Mandatory | 1 | 0 |
| CWE-662: Improper Synchronization | Potential | 8 | [1](#CWE-662_Improper_Synchronization) |
| CWE-820: Missing Synchronization | Potential | 8 | [1](#CWE-820_Missing_Synchronization) |
| CWE-567: Unsynchronized Access to Shared Data in a Multithreaded Context | Potential | 5 | [1](#CWE-567_Unsynchronized_Access_to_Shared_Data_in_a_Multithreaded_Context) |
| CWE-99: Improper Control of Resource Identifiers ('Resource Injection') | Potential | 3 | [1](#CWE-99_Improper_Control_of_Resource_Identifiers_Resource_Injection) |
| CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting') | Optional | 8 | [1](#CWE-79_Improper_Neutralization_of_Input_During_Web_Page_Generation_Cross-site_Scripting) |
| CWE-798: Use of Hard-coded Credentials | Optional | 5 | [1](#CWE-798_Use_of_Hard-coded_Credentials) |
| GHSA-72hv-8253-57qq: jackson-core: Number Length Constraint Bypass in Async Parser Leads to Potential DoS Condition | Optional | 1 | 0 |
| CVE-2025-11226: QOS.CH logback-core is vulnerable to Arbitrary Code Execution through file processing | Optional | 1 | 0 |
| CVE-2024-12798: QOS.CH logback-core Expression Language Injection vulnerability | Optional | 1 | 0 |
| CVE-2025-48924: Apache Commons Lang is vulnerable to Uncontrolled Recursion when processing long inputs | Optional | 1 | 0 |
| CVE-2026-42585: Netty vulnerable to HTTP Request Smuggling due to malformed Transfer-Encoding | Optional | 1 | 0 |
| CVE-2026-42581: Netty HTTP/1.0 TE+CL Coexistence Bypasses Smuggling Sanitization | Optional | 1 | 0 |
| CVE-2026-42580: Netty vulnerable to HTTP Request Smuggling due to incorrect chunk size parsing | Optional | 1 | 0 |
| CVE-2026-41417: Netty: Start-Line Injection in DefaultHttpRequest.setUri() Allows HTTP Request Smuggling and RTSP Request Injection | Optional | 1 | 0 |
| CVE-2025-67735: Netty has a CRLF Injection vulnerability in io.netty.handler.codec.http.HttpRequestEncoder | Optional | 1 | 0 |
| CVE-2025-58057: Netty's decoders vulnerable to DoS via zip bomb style attack | Optional | 1 | 0 |
| CVE-2025-25193: Denial of Service attack on windows app using Netty | Optional | 1 | 0 |
| CVE-2026-45292: OpenTelemetry Java SDK has Unbounded Memory Allocation in W3C Baggage Propagation | Optional | 1 | 0 |
| CVE-2025-22227: Reactor Netty HTTP is vulnerable to credential leaks during chained redirects | Optional | 1 | 0 |
| CVE-2020-36843: Ed25519 Signature Malleability in ed25519-java Due to Missing Scalar Range Check | Optional | 1 | 0 |
| CVE-2026-0636: Bouncy Castle has an LDAP injection | Optional | 1 | 0 |
| CVE-2026-25854: Apache Tomcat has an Open Redirect vulnerability | Optional | 1 | 0 |
| CVE-2025-66614: Apache Tomcat - Client certificate verification bypass | Optional | 1 | 0 |
| CVE-2025-49124: Apache Tomcat installer for Windows has an untrusted search path vulnerability | Optional | 1 | 0 |
| CVE-2025-49125: Apache Tomcat - Security constraint bypass for pre/post-resources | Optional | 1 | 0 |
| CVE-2025-31650: Apache Tomcat Denial of Service via invalid HTTP priority header | Optional | 1 | 0 |
| CVE-2020-13956: Cross-site scripting in Apache HttpClient | Optional | 1 | 0 |
| CVE-2025-4949: Eclipse JGit XML External Entity (XXE) Vulnerability | Optional | 1 | 0 |
| CVE-2026-41004: Spring Cloud Config Server Logged Sensitive Information | Optional | 1 | [1](#CVE-2026-41004_Spring_Cloud_Config_Server_Logged_Sensitive_Information) |
| CVE-2026-22745: Spring MVC and WebFlux applications are vulnerable to Denial of Service attacks when resolving static resources | Optional | 1 | 0 |
| CVE-2026-22737: Spring Framework Improper Path Limitation with Script View Templates | Optional | 1 | 0 |
| CVE-2025-41242: Spring Framework MVC Applications Path Traversal Vulnerability | Optional | 1 | 0 |
| CVE-2025-41234: Spring Framework vulnerable to a reflected file download (RFD) | Optional | 1 | 0 |

### Security Issue Details

<details id="CVE-2026-40982_Spring_Cloud_Config_vulnerable_to_Path_Traversal">
<summary><b>CVE-2026-40982: Spring Cloud Config vulnerable to Path Traversal</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml:31`

</details>

<details id="CVE-2026-40972_Spring_Boot_DevTools_remote_secret_comparison_is_vulnerable_to_timing_attacks">
<summary><b>CVE-2026-40972: Spring Boot DevTools remote secret comparison is vulnerable to timing attacks</b> — affected files</summary>

- `spring-petclinic-api-gateway/pom.xml:32`

</details>

<details id="CVE-2026-22733_Spring_Boot_has_an_Authentication_Bypass_under_Actuator_CloudFoundry_endpoints">
<summary><b>CVE-2026-22733: Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints</b> — affected files</summary>

- `spring-petclinic-api-gateway/pom.xml:42`
- `spring-petclinic-customers-service/pom.xml:25`
- `spring-petclinic-genai-service/pom.xml:39`
- `spring-petclinic-vets-service/pom.xml:33`
- `spring-petclinic-visits-service/pom.xml:24`

</details>

<details id="CVE-2026-22731_Spring_Boot_has_an_Authentication_Bypass_under_Actuator_Health_groups_paths">
<summary><b>CVE-2026-22731: Spring Boot has an Authentication Bypass under Actuator Health groups paths</b> — affected files</summary>

- `spring-petclinic-api-gateway/pom.xml:42`
- `spring-petclinic-customers-service/pom.xml:25`
- `spring-petclinic-genai-service/pom.xml:39`
- `spring-petclinic-vets-service/pom.xml:33`
- `spring-petclinic-visits-service/pom.xml:24`

</details>

<details id="CVE-2026-41002_Spring_Cloud_Config_Server_Susceptible_To_TOCTOU_Attack">
<summary><b>CVE-2026-41002: Spring Cloud Config Server Susceptible To TOCTOU Attack</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml:31`

</details>

<details id="CVE-2026-22739_Spring_Cloud_Config_Server_Path_Traversal_via_Profile_Parameter_Allows_Arbitrary_File_Access">
<summary><b>CVE-2026-22739: Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml:31`

</details>

<details id="CWE-662_Improper_Synchronization">
<summary><b>CWE-662: Improper Synchronization</b> — affected files</summary>

- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java`

</details>

<details id="CWE-820_Missing_Synchronization">
<summary><b>CWE-820: Missing Synchronization</b> — affected files</summary>

- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java`

</details>

<details id="CWE-567_Unsynchronized_Access_to_Shared_Data_in_a_Multithreaded_Context">
<summary><b>CWE-567: Unsynchronized Access to Shared Data in a Multithreaded Context</b> — affected files</summary>

- `spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java`

</details>

<details id="CWE-99_Improper_Control_of_Resource_Identifiers_Resource_Injection">
<summary><b>CWE-99: Improper Control of Resource Identifiers ('Resource Injection')</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/AIDataProvider.java`

</details>

<details id="CWE-79_Improper_Neutralization_of_Input_During_Web_Page_Generation_Cross-site_Scripting">
<summary><b>CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/PetclinicChatClient.java`

</details>

<details id="CWE-798_Use_of_Hard-coded_Credentials">
<summary><b>CWE-798: Use of Hard-coded Credentials</b> — affected files</summary>

- `spring-petclinic-genai-service/src/main/resources/application.yml`

</details>

<details id="CVE-2026-41004_Spring_Cloud_Config_Server_Logged_Sensitive_Information">
<summary><b>CVE-2026-41004: Spring Cloud Config Server Logged Sensitive Information</b> — affected files</summary>

- `spring-petclinic-config-server/pom.xml:31`

</details>

---

## Codebase Insights

> **Note:** These documents are generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

> **Codebase Insights aren't available yet.**
>
> These documents are generated when assessment runs with **Full analysis** coverage. Re-run the assessment and set `analysisCoverage: full` to enable them.

[Share feedback](https://aka.ms/ghcp-appmod/feedback)
