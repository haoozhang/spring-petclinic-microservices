# Security Assessment Report

**Generated:** 2026-04-10T08:28:00Z

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 8 |
| CVE Vulnerabilities | 3 |
| CWE Vulnerabilities | 5 |
| Total Rules Assessed | 59 |
| Rules Passed | 54 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 3 |
| optional | 3 |
| potential | 2 |

### By Category

| Category | Count |
|----------|-------|
| CVE | 3 |
| Code Quality | 2 |
| Credentials & Secrets | 2 |
| Injection Attacks | 1 |

## CVE Findings (Dependency Vulnerabilities)

### CVE-2026-22739: Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access

- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-config-server/pom.xml:33

[CVE-2026-22739](https://github.com/advisories/GHSA-3qwq-q9vm-5j42): Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access

Severity: MANDATORY (high)

Affected dependencies:
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:33)
    Vulnerable range: >= 4.2.0, <= 4.2.4

Note: No patched version available in the 4.2.x line at time of assessment. Consider upgrading to the 4.3.x line (patched at 4.3.2) or the 5.0.x line (patched at 5.0.2).

### CVE-2026-22733: Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints

- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-api-gateway/pom.xml:44, spring-petclinic-customers-service/pom.xml:27, spring-petclinic-genai-service/pom.xml:41, spring-petclinic-vets-service/pom.xml:35, spring-petclinic-visits-service/pom.xml:26

[CVE-2026-22733](https://github.com/advisories/GHSA-mgvc-8q2h-5pgc): Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints

Severity: MANDATORY (high)

Affected dependencies:
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-api-gateway/pom.xml:44, spring-petclinic-customers-service/pom.xml:27, spring-petclinic-genai-service/pom.xml:41, spring-petclinic-vets-service/pom.xml:35, spring-petclinic-visits-service/pom.xml:26)
    Vulnerable range: >= 3.4.0, <= 3.4.13

Note: No patched version available in the 3.4.x line at time of assessment. Consider upgrading to Spring Boot 3.5.12 or later.

### CVE-2026-22731: Spring Boot has an Authentication Bypass under Actuator Health groups paths

- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-api-gateway/pom.xml:44, spring-petclinic-customers-service/pom.xml:27, spring-petclinic-genai-service/pom.xml:41, spring-petclinic-vets-service/pom.xml:35, spring-petclinic-visits-service/pom.xml:26

[CVE-2026-22731](https://github.com/advisories/GHSA-8hfc-fq58-r658): Spring Boot has an Authentication Bypass under Actuator Health groups paths

Severity: MANDATORY (high)

Affected dependencies:
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-api-gateway/pom.xml:44, spring-petclinic-customers-service/pom.xml:27, spring-petclinic-genai-service/pom.xml:41, spring-petclinic-vets-service/pom.xml:35, spring-petclinic-visits-service/pom.xml:26)
    Vulnerable range: >= 3.4.0, <= 3.4.13

Note: No patched version available in the 3.4.x line at time of assessment. Consider upgrading to Spring Boot 3.5.12 or later.

## CWE Findings (Code-Level Vulnerabilities)

### CWE-665: Improper Initialization

- **Category:** Code Quality
- **Severity:** potential
- **Story Points:** 3
- **Files:** spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/VectorStoreController.java

In VectorStoreController, the method convertListToJsonResource() (line 94) returns null when a JsonProcessingException occurs (line 108). The caller loadVetDataToVectorStoreOnStartup() uses the return value on line 76 (Resource vetsAsJson = convertListToJsonResource(vets)) and immediately passes it to new JsonReader(vetsAsJson) on line 77 without any null check. If JSON serialization fails, vetsAsJson will be null, causing a NullPointerException when JsonReader tries to access the resource, leading to an improperly initialized reader object.

### CWE-1057: Data Access Operations Outside of Expected Data Manager Component

- **Category:** Code Quality
- **Severity:** potential
- **Story Points:** 5
- **Files:** spring-petclinic-customers-service/src/main/java/org/springframework/samples/petclinic/customers/web/OwnerResource.java, spring-petclinic-customers-service/src/main/java/org/springframework/samples/petclinic/customers/web/PetResource.java, spring-petclinic-vets-service/src/main/java/org/springframework/samples/petclinic/vets/web/VetResource.java, spring-petclinic-visits-service/src/main/java/org/springframework/samples/petclinic/visits/web/VisitResource.java

The REST controller classes (OwnerResource, PetResource, VetResource, VisitResource) directly inject and call JPA Repository interfaces (OwnerRepository, PetRepository, VetRepository, VisitRepository) instead of routing data access through a dedicated service layer. For example, OwnerResource (line 46) directly injects OwnerRepository and calls ownerRepository.save(), ownerRepository.findById(), and ownerRepository.findAll() (lines 61, 69, 77, 86, 90). This bypasses the expected data manager (service) component and couples the presentation layer directly to the data access layer.

### CWE-259: Use of Hard-coded Password

- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** README.md, spring-petclinic-genai-service/src/main/resources/application.yml

Two instances found: (1) README.md line 151 contains a docker run command with a hardcoded MySQL root password: 'docker run -e MYSQL_ROOT_PASSWORD=petclinic -e MYSQL_DATABASE=petclinic'. This documents using 'petclinic' as the database root password, which is a well-known default credential that should not be used in any environment. (2) application.yml line 25: 'api-key: ${OPENAI_API_KEY:demo}' uses 'demo' as a hardcoded fallback value for the OpenAI API key, allowing the application to silently continue with an invalid/placeholder credential if the environment variable is not set.

### CWE-798: Use of Hard-coded Credentials

- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** README.md, spring-petclinic-genai-service/src/main/resources/application.yml

Same findings as CWE-259: (1) README.md line 151 hardcodes 'petclinic' as the MySQL root password and database name in a documented docker run command, establishing a well-known default credential for the database. (2) application.yml line 25 hardcodes 'demo' as the fallback value for ${OPENAI_API_KEY:demo}, meaning if the OPENAI_API_KEY environment variable is absent, the application uses a hardcoded placeholder credential that may expose API calls or cause silent failures.

### CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')

- **Category:** Injection Attacks
- **Severity:** optional
- **Story Points:** 8
- **Files:** spring-petclinic-api-gateway/src/main/resources/static/scripts/genai/chat.js

In chat.js, user-supplied chat input (line 39: appendMessage(query, 'user')) and AI server responses (line 52: appendMessage(responseText, 'bot')) are both rendered via messageElement.innerHTML = htmlContent (line 8) after passing through marked.parse() without sanitization. marked.parse() by default does not strip script tags or event handlers, so malicious input can execute arbitrary JavaScript. Additionally, chat history is persisted to localStorage as raw innerHTML (line 70) and restored via innerHTML (line 78), enabling stored XSS across page reloads.
