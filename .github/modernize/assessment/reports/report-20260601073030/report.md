# spring-petclinic-microservices

## Summary

| Metric | Value |
|--------|-------|
| Total Issues | 42 |
| Mandatory Blockers | 31 |
| Potential Issues | 8 |

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
| Server port configuration found | Potential | 1 | [1](#Server_port_configuration_found) |
| Restricted configurations found | Potential | 2 | [1](#Restricted_configurations_found) |
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

- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 25)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 24)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 26)`
- `spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java (line 27)`

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

- `spring-petclinic-genai-service/pom.xml (line 120)`
- `spring-petclinic-genai-service/pom.xml (line 124)`
- `spring-petclinic-genai-service/pom.xml (line 112)`
- `spring-petclinic-api-gateway/pom.xml (line 97)`
- `spring-petclinic-api-gateway/pom.xml (line 101)`
- `spring-petclinic-api-gateway/pom.xml (line 89)`
- `spring-petclinic-customers-service/pom.xml (line 86)`
- `spring-petclinic-customers-service/pom.xml (line 78)`
- `spring-petclinic-customers-service/pom.xml (line 90)`
- `spring-petclinic-vets-service/pom.xml (line 106)`
- `spring-petclinic-vets-service/pom.xml (line 98)`
- `spring-petclinic-vets-service/pom.xml (line 110)`
- `spring-petclinic-visits-service/pom.xml (line 77)`
- `spring-petclinic-visits-service/pom.xml (line 85)`
- `spring-petclinic-visits-service/pom.xml (line 89)`

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

<details id="Server_port_configuration_found">
<summary><b>Server port configuration found</b> — affected files</summary>

- `spring-petclinic-config-server/src/main/resources/application.yml (line 1)`

</details>

<details id="Restricted_configurations_found">
<summary><b>Restricted configurations found</b> — affected files</summary>

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

## Security Issues

> **Note:** These issues were generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

| Issue Name | Criticality | Story Points | Files |
|------------|-------------|--------------|-------|
| CVE-2016-1000027: Pivotal Spring Framework contains unsafe Java deserialization methods | Mandatory | 1 | [1](#CVE-2016-1000027_Pivotal_Spring_Framework_contains_unsafe_Java_deserialization_methods) |
| CVE-2017-5929: QOS.ch Logback vulnerable to Deserialization of Untrusted Data | Mandatory | 1 | [1](#CVE-2017-5929_QOS_ch_Logback_vulnerable_to_Deserialization_of_Untrusted_Data) |
| CVE-2019-17267: Improper Input Validation in jackson-databind | Mandatory | 1 | [1](#CVE-2019-17267_Improper_Input_Validation_in_jackson-databind) |
| CVE-2019-17531: jackson-databind polymorphic typing issue | Mandatory | 1 | [1](#CVE-2019-17531_jackson-databind_polymorphic_typing_issue) |
| CVE-2019-16943: jackson-databind polymorphic typing issue | Mandatory | 1 | [1](#CVE-2019-16943_jackson-databind_polymorphic_typing_issue) |
| CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-16335_Polymorphic_Typing_issue_in_FasterXML_jackson-databind) |
| CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-14540_Polymorphic_Typing_issue_in_FasterXML_jackson-databind) |
| CVE-2019-14379: Deserialization of untrusted data in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-14379_Deserialization_of_untrusted_data_in_FasterXML_jackson-databind) |
| CVE-2013-7285: Command Injection in Xstream | Mandatory | 1 | [1](#CVE-2013-7285_Command_Injection_in_Xstream) |
| CVE-2017-17485: jackson-databind vulnerable to remote code execution due to incorrect deserialization and blocklist bypass | Mandatory | 1 | [1](#CVE-2017-17485_jackson-databind_vulnerable_to_remote_code_execution_due_to_incorrect_deserialization_and_blocklist_bypass) |
| CVE-2018-7489: FasterXML jackson-databind allows unauthenticated remote code execution  | Mandatory | 1 | [1](#CVE-2018-7489_FasterXML_jackson-databind_allows_unauthenticated_remote_code_execution) |
| CVE-2017-7525: jackson-databind is vulnerable to a deserialization flaw | Mandatory | 1 | [1](#CVE-2017-7525_jackson-databind_is_vulnerable_to_a_deserialization_flaw) |
| CVE-2022-22965: Remote Code Execution in Spring Framework | Mandatory | 1 | [2](#CVE-2022-22965_Remote_Code_Execution_in_Spring_Framework) |
| CVE-2019-20444: HTTP Request Smuggling in Netty | Mandatory | 1 | [1](#CVE-2019-20444_HTTP_Request_Smuggling_in_Netty) |
| CVE-2026-41901: Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns | Mandatory | 1 | [1](#CVE-2026-41901_Sandboxed_Thymeleaf_expressions_vulnerable_to_improper_recognition_of_unauthorized_syntax_patterns) |
| CVE-2026-40478: Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf | Mandatory | 1 | [1](#CVE-2026-40478_Improper_neutralization_of_specific_syntax_patterns_for_unauthorized_expressions_in_Thymeleaf) |
| CVE-2026-40477: Improper restriction of the scope of accessible objects in Thymeleaf expressions | Mandatory | 1 | [1](#CVE-2026-40477_Improper_restriction_of_the_scope_of_accessible_objects_in_Thymeleaf_expressions) |
| CVE-2023-20873: Spring Boot Security Bypass with Wildcard Pattern Matching on Cloud Foundry | Mandatory | 1 | [1](#CVE-2023-20873_Spring_Boot_Security_Bypass_with_Wildcard_Pattern_Matching_on_Cloud_Foundry) |
| CVE-2026-43512: Apache Tomcat - Digest authenticator will authenticate any unknown user | Mandatory | 1 | [1](#CVE-2026-43512_Apache_Tomcat_-_Digest_authenticator_will_authenticate_any_unknown_user) |
| CVE-2026-43515: Apache Tomcat - Security constraints not correctly applied | Mandatory | 1 | [1](#CVE-2026-43515_Apache_Tomcat_-_Security_constraints_not_correctly_applied) |
| CVE-2026-41293: Apache Tomcat - HTTP/2 request headers not validated | Mandatory | 1 | [1](#CVE-2026-41293_Apache_Tomcat_-_HTTP_2_request_headers_not_validated) |
| CVE-2022-41853: HyperSQL DataBase vulnerable to remote code execution when processing untrusted input | Mandatory | 1 | [1](#CVE-2022-41853_HyperSQL_DataBase_vulnerable_to_remote_code_execution_when_processing_untrusted_input) |
| CVE-2018-1275: Spring Framework has Improperly Implemented Security Check for Standard | Mandatory | 1 | [1](#CVE-2018-1275_Spring_Framework_has_Improperly_Implemented_Security_Check_for_Standard) |
| CVE-2018-1270: Spring Framework allows applications to expose STOMP over WebSocket endpoints | Mandatory | 1 | [1](#CVE-2018-1270_Spring_Framework_allows_applications_to_expose_STOMP_over_WebSocket_endpoints) |
| CVE-2014-9390: JGit Improper Input Validation vulnerability | Mandatory | 1 | [1](#CVE-2014-9390_JGit_Improper_Input_Validation_vulnerability) |
| CVE-2016-3720: jackson-dataformat-xml vulnerable to XML external entity (XXE) | Mandatory | 1 | [1](#CVE-2016-3720_jackson-dataformat-xml_vulnerable_to_XML_external_entity_XXE) |

### Security Issue Details

<details id="CVE-2016-1000027_Pivotal_Spring_Framework_contains_unsafe_Java_deserialization_methods">
<summary><b>CVE-2016-1000027: Pivotal Spring Framework contains unsafe Java deserialization methods</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2017-5929_QOS_ch_Logback_vulnerable_to_Deserialization_of_Untrusted_Data">
<summary><b>CVE-2017-5929: QOS.ch Logback vulnerable to Deserialization of Untrusted Data</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-17267_Improper_Input_Validation_in_jackson-databind">
<summary><b>CVE-2019-17267: Improper Input Validation in jackson-databind</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-17531_jackson-databind_polymorphic_typing_issue">
<summary><b>CVE-2019-17531: jackson-databind polymorphic typing issue</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-16943_jackson-databind_polymorphic_typing_issue">
<summary><b>CVE-2019-16943: jackson-databind polymorphic typing issue</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-16335_Polymorphic_Typing_issue_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-14540_Polymorphic_Typing_issue_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2019-14379_Deserialization_of_untrusted_data_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-14379: Deserialization of untrusted data in FasterXML jackson-databind</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2013-7285_Command_Injection_in_Xstream">
<summary><b>CVE-2013-7285: Command Injection in Xstream</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2017-17485_jackson-databind_vulnerable_to_remote_code_execution_due_to_incorrect_deserialization_and_blocklist_bypass">
<summary><b>CVE-2017-17485: jackson-databind vulnerable to remote code execution due to incorrect deserialization and blocklist bypass</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2018-7489_FasterXML_jackson-databind_allows_unauthenticated_remote_code_execution">
<summary><b>CVE-2018-7489: FasterXML jackson-databind allows unauthenticated remote code execution </b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2017-7525_jackson-databind_is_vulnerable_to_a_deserialization_flaw">
<summary><b>CVE-2017-7525: jackson-databind is vulnerable to a deserialization flaw</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2022-22965_Remote_Code_Execution_in_Spring_Framework">
<summary><b>CVE-2022-22965: Remote Code Execution in Spring Framework</b> — affected files</summary>

- `pom.xml`
- `pom.xml:7`

</details>

<details id="CVE-2019-20444_HTTP_Request_Smuggling_in_Netty">
<summary><b>CVE-2019-20444: HTTP Request Smuggling in Netty</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2026-41901_Sandboxed_Thymeleaf_expressions_vulnerable_to_improper_recognition_of_unauthorized_syntax_patterns">
<summary><b>CVE-2026-41901: Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2026-40478_Improper_neutralization_of_specific_syntax_patterns_for_unauthorized_expressions_in_Thymeleaf">
<summary><b>CVE-2026-40478: Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2026-40477_Improper_restriction_of_the_scope_of_accessible_objects_in_Thymeleaf_expressions">
<summary><b>CVE-2026-40477: Improper restriction of the scope of accessible objects in Thymeleaf expressions</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2023-20873_Spring_Boot_Security_Bypass_with_Wildcard_Pattern_Matching_on_Cloud_Foundry">
<summary><b>CVE-2023-20873: Spring Boot Security Bypass with Wildcard Pattern Matching on Cloud Foundry</b> — affected files</summary>

- `pom.xml:7`

</details>

<details id="CVE-2026-43512_Apache_Tomcat_-_Digest_authenticator_will_authenticate_any_unknown_user">
<summary><b>CVE-2026-43512: Apache Tomcat - Digest authenticator will authenticate any unknown user</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2026-43515_Apache_Tomcat_-_Security_constraints_not_correctly_applied">
<summary><b>CVE-2026-43515: Apache Tomcat - Security constraints not correctly applied</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2026-41293_Apache_Tomcat_-_HTTP_2_request_headers_not_validated">
<summary><b>CVE-2026-41293: Apache Tomcat - HTTP/2 request headers not validated</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2022-41853_HyperSQL_DataBase_vulnerable_to_remote_code_execution_when_processing_untrusted_input">
<summary><b>CVE-2022-41853: HyperSQL DataBase vulnerable to remote code execution when processing untrusted input</b> — affected files</summary>

- `spring-petclinic-vets-service/pom.xml:79`

</details>

<details id="CVE-2018-1275_Spring_Framework_has_Improperly_Implemented_Security_Check_for_Standard">
<summary><b>CVE-2018-1275: Spring Framework has Improperly Implemented Security Check for Standard</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2018-1270_Spring_Framework_allows_applications_to_expose_STOMP_over_WebSocket_endpoints">
<summary><b>CVE-2018-1270: Spring Framework allows applications to expose STOMP over WebSocket endpoints</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2014-9390_JGit_Improper_Input_Validation_vulnerability">
<summary><b>CVE-2014-9390: JGit Improper Input Validation vulnerability</b> — affected files</summary>

- `pom.xml`

</details>

<details id="CVE-2016-3720_jackson-dataformat-xml_vulnerable_to_XML_external_entity_XXE">
<summary><b>CVE-2016-3720: jackson-dataformat-xml vulnerable to XML external entity (XXE)</b> — affected files</summary>

- `pom.xml`

</details>

---

## Codebase Insights

> **Note:** These documents are generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

> **Codebase Insights aren't available yet.**
>
> These documents are generated when assessment runs with **Full analysis** coverage. Re-run the assessment and set `analysisCoverage: full` to enable them.

[Share feedback](https://aka.ms/ghcp-appmod/feedback)
