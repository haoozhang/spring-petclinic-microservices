# Security Assessment Report

**Generated:** 2026-06-01T07:37:50.0000000Z

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 26 |
| CVE Vulnerabilities | 26 |
| CWE Vulnerabilities | 0 |
| Total Rules Assessed | 59 |
| Rules Passed | 59 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 26 |
| optional | 0 |
| potential | 0 |

## CVE Findings (Dependency Vulnerabilities)

### CVE-2016-1000027: Pivotal Spring Framework contains unsafe Java deserialization methods
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2016-1000027](https://github.com/advisories): Pivotal Spring Framework contains unsafe Java deserialization methods

Severity: CRITICAL

Affected dependencies:
  - org.springframework:spring-web (< 6.0.0) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 6.0.0

### CVE-2017-5929: QOS.ch Logback vulnerable to Deserialization of Untrusted Data
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2017-5929](https://github.com/advisories): QOS.ch Logback vulnerable to Deserialization of Untrusted Data

Severity: CRITICAL

Affected dependencies:
  - ch.qos.logback:logback-classic (< 1.2.0) (declared at pom.xml)
  - ch.qos.logback:logback-core (< 1.2.0) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 1.2.0

### CVE-2019-17267: Improper Input Validation in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-17267](https://github.com/advisories): Improper Input Validation in jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.10) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.8.11.5) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.8.11.5, 2.9.10

### CVE-2019-17531: jackson-databind polymorphic typing issue
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-17531](https://github.com/advisories): jackson-databind polymorphic typing issue

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.10.1) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, < 2.8.11.5) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.6.7.3) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.3, 2.8.11.5, 2.9.10.1

### CVE-2019-16943: jackson-databind polymorphic typing issue
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-16943](https://github.com/advisories): jackson-databind polymorphic typing issue

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.10.1) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, < 2.8.11.5) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.6.7.3) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.3, 2.8.11.5, 2.9.10.1

### CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-16335](https://github.com/advisories): Polymorphic Typing issue in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.10) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, < 2.8.11.5) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.6.7.3) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.3, 2.8.11.5, 2.9.10

### CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-14540](https://github.com/advisories): Polymorphic Typing issue in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.10) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, < 2.8.11.5) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.6.7.3) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.3, 2.8.11.5, 2.9.10

### CVE-2019-14379: Deserialization of untrusted data in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-14379](https://github.com/advisories): Deserialization of untrusted data in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.9.2) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.8.0, < 2.8.11.4) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.7.9.6) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.7.9.6, 2.8.11.4, 2.9.9.2

### CVE-2013-7285: Command Injection in Xstream
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2013-7285](https://github.com/advisories): Command Injection in Xstream

Severity: CRITICAL

Affected dependencies:
  - com.thoughtworks.xstream:xstream (< 1.4.7) (declared at pom.xml)
  - com.thoughtworks.xstream:xstream (= 1.4.10) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 1.4.11, 1.4.7

### CVE-2017-17485: jackson-databind vulnerable to remote code execution due to incorrect deserialization and blocklist bypass
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2017-17485](https://github.com/advisories): jackson-databind vulnerable to remote code execution due to incorrect deserialization and blocklist bypass

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.4) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.8.0, < 2.8.11) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.7.9.2) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.7.9.2, 2.8.11, 2.9.4

### CVE-2018-7489: FasterXML jackson-databind allows unauthenticated remote code execution 
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2018-7489](https://github.com/advisories): FasterXML jackson-databind allows unauthenticated remote code execution 

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.9.0, < 2.9.5) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.8.0, <= 2.8.11.0) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, < 2.7.9.3) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (< 2.6.7.5) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.5, 2.7.9.3, 2.8.11.1, 2.9.5

### CVE-2017-7525: jackson-databind is vulnerable to a deserialization flaw
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2017-7525](https://github.com/advisories): jackson-databind is vulnerable to a deserialization flaw

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind (>= 2.8.0, < 2.8.9) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (<= 2.6.7.0) (declared at pom.xml)
  - com.fasterxml.jackson.core:jackson-databind (>= 2.7.0, <= 2.7.9.0) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.6.7.1, 2.7.9.1, 2.8.9

### CVE-2022-22965: Remote Code Execution in Spring Framework
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml, pom.xml:7

[CVE-2022-22965](https://github.com/advisories): Remote Code Execution in Spring Framework

Severity: CRITICAL

Affected dependencies:
  - org.springframework:spring-beans (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework:spring-webmvc (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-web (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-web (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-webflux (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-webflux (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-webflux (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-beans (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webmvc (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webflux (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-beans (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework:spring-webmvc (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-web (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-web (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-webflux (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-webflux (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-webflux (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-beans (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webmvc (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webflux (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-beans (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework:spring-webmvc (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-web (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-web (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-webflux (>= 5.3.0, < 5.3.18) (declared at pom.xml)
  - org.springframework.boot:spring-boot-starter-webflux (< 2.5.12) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-starter-webflux (>= 2.6.0, < 2.6.6) (declared at pom.xml:7)
  - org.springframework:spring-beans (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webmvc (< 5.2.20.RELEASE) (declared at pom.xml)
  - org.springframework:spring-webflux (< 5.2.20.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.5.12, 2.6.6, 5.2.20.RELEASE, 5.3.18

### CVE-2019-20444: HTTP Request Smuggling in Netty
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2019-20444](https://github.com/advisories): HTTP Request Smuggling in Netty

Severity: CRITICAL

Affected dependencies:
  - org.jboss.netty:netty (< 4.0.0) (declared at pom.xml)
  - io.netty:netty (< 4.0.0) (declared at pom.xml)
  - io.netty:netty-codec-http (< 4.1.44) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 4.1.44

### CVE-2026-41901: Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-41901](https://github.com/advisories): Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf (<= 3.1.4.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring5 (<= 3.1.4.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring6 (<= 3.1.4.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 3.1.5.RELEASE

### CVE-2026-40478: Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-40478](https://github.com/advisories): Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf (<= 3.1.3.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring5 (<= 3.1.3.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring6 (<= 3.1.3.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 3.1.4.RELEASE

### CVE-2026-40477: Improper restriction of the scope of accessible objects in Thymeleaf expressions
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-40477](https://github.com/advisories): Improper restriction of the scope of accessible objects in Thymeleaf expressions

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf (<= 3.1.3.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring5 (<= 3.1.3.RELEASE) (declared at pom.xml)
  - org.thymeleaf:thymeleaf-spring6 (<= 3.1.3.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 3.1.4.RELEASE

### CVE-2023-20873: Spring Boot Security Bypass with Wildcard Pattern Matching on Cloud Foundry
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml:7

[CVE-2023-20873](https://github.com/advisories): Spring Boot Security Bypass with Wildcard Pattern Matching on Cloud Foundry

Severity: CRITICAL

Affected dependencies:
  - org.springframework.boot:spring-boot-actuator-autoconfigure (>= 3.0.0, < 3.0.6) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-actuator-autoconfigure (>= 2.7.0, < 2.7.11) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-actuator-autoconfigure (>= 2.6.0, < 2.6.15) (declared at pom.xml:7)
  - org.springframework.boot:spring-boot-actuator-autoconfigure (< 2.5.15) (declared at pom.xml:7)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.5.15, 2.6.15, 2.7.11, 3.0.6

### CVE-2026-43512: Apache Tomcat - Digest authenticator will authenticate any unknown user
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-43512](https://github.com/advisories): Apache Tomcat - Digest authenticator will authenticate any unknown user

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 10.1.55, 11.0.22, 9.0.118

### CVE-2026-43515: Apache Tomcat - Security constraints not correctly applied
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-43515](https://github.com/advisories): Apache Tomcat - Security constraints not correctly applied

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 10.1.55, 11.0.22, 9.0.118

### CVE-2026-41293: Apache Tomcat - HTTP/2 request headers not validated
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2026-41293](https://github.com/advisories): Apache Tomcat - HTTP/2 request headers not validated

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat.embed:tomcat-embed-core (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (< 9.0.118) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 10.1.0-M1, < 10.1.55) (declared at pom.xml)
  - org.apache.tomcat:tomcat-catalina (>= 11.0.0-M1, < 11.0.22) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 10.1.55, 11.0.22, 9.0.118

### CVE-2022-41853: HyperSQL DataBase vulnerable to remote code execution when processing untrusted input
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-vets-service/pom.xml:79

[CVE-2022-41853](https://github.com/advisories): HyperSQL DataBase vulnerable to remote code execution when processing untrusted input

Severity: CRITICAL

Affected dependencies:
  - org.hsqldb:hsqldb (< 2.7.1) (declared at spring-petclinic-vets-service/pom.xml:79)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.7.1

### CVE-2018-1275: Spring Framework has Improperly Implemented Security Check for Standard
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2018-1275](https://github.com/advisories): Spring Framework has Improperly Implemented Security Check for Standard

Severity: CRITICAL

Affected dependencies:
  - org.springframework:spring-messaging (< 4.3.16.RELEASE) (declared at pom.xml)
  - org.springframework:spring-messaging (>= 5.0.0.RELEASE, < 5.0.5.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 4.3.16.RELEASE, 5.0.5.RELEASE

### CVE-2018-1270: Spring Framework allows applications to expose STOMP over WebSocket endpoints
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2018-1270](https://github.com/advisories): Spring Framework allows applications to expose STOMP over WebSocket endpoints

Severity: CRITICAL

Affected dependencies:
  - org.springframework:spring-messaging (>= 5.0.0.RELEASE, < 5.0.5.RELEASE) (declared at pom.xml)
  - org.springframework:spring-messaging (< 4.3.16.RELEASE) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 4.3.16.RELEASE, 5.0.5.RELEASE

### CVE-2014-9390: JGit Improper Input Validation vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2014-9390](https://github.com/advisories): JGit Improper Input Validation vulnerability

Severity: CRITICAL

Affected dependencies:
  - org.eclipse.jgit:org.eclipse.jgit (< 3.5.3) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 3.5.3

### CVE-2016-3720: jackson-dataformat-xml vulnerable to XML external entity (XXE)
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** pom.xml

[CVE-2016-3720](https://github.com/advisories): jackson-dataformat-xml vulnerable to XML external entity (XXE)

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.dataformat:jackson-dataformat-xml (< 2.7.4) (declared at pom.xml)

Recommended fix:
  - Upgrade affected dependencies to patched versions such as 2.7.4

## CWE Findings (Code-Level Vulnerabilities)

No CWE findings were reported.
