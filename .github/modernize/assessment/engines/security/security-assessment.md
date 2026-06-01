# Security Assessment Report

**Generated:** 2026-06-01T04:00:42.0000000Z

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 76 |
| CVE Vulnerabilities | 70 |
| CWE Vulnerabilities | 6 |
| Total Rules Assessed | 59 |
| Rules Passed | 53 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 43 |
| optional | 29 |
| potential | 4 |

## CVE Findings (Dependency Vulnerabilities)

### CVE-2026-43512: Apache Tomcat - Digest authenticator will authenticate any unknown user
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-43512](https://github.com/advisories/GHSA-h6fc-48rj-7qqh): Apache Tomcat - Digest authenticator will authenticate any unknown user

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2026-43515: Apache Tomcat - Security constraints not correctly applied
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-43515](https://github.com/advisories/GHSA-5m62-pw8w-7w9f): Apache Tomcat - Security constraints not correctly applied

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2026-41293: Apache Tomcat - HTTP/2 request headers not validated
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-41293](https://github.com/advisories/GHSA-r29c-68gh-xp6x): Apache Tomcat - HTTP/2 request headers not validated

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2025-24813: Apache Tomcat: Potential RCE and/or information disclosure and/or information corruption with partial PUT
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-24813](https://github.com/advisories/GHSA-83qj-6fr2-vhqg): Apache Tomcat: Potential RCE and/or information disclosure and/or information corruption with partial PUT

Severity: CRITICAL

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.3 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.35 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.99 or later

### CVE-2025-12383: Eclipse Jersey has a Race Condition
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-12383](https://github.com/advisories/GHSA-7p63-w6x9-6gr7): Eclipse Jersey has a Race Condition

Severity: CRITICAL

Affected dependencies:
  - org.glassfish.jersey.core:jersey-client:3.1.9 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.glassfish.jersey.core:jersey-client to 3.1.10 or later

### CVE-2026-40982: Spring Cloud Config vulnerable to Path Traversal
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-config-server/pom.xml:31

[CVE-2026-40982](https://github.com/advisories/GHSA-6g23-24mc-hx6x): Spring Cloud Config vulnerable to Path Traversal

Severity: CRITICAL

Affected dependencies:
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:31)

### CVE-2026-41901: Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-41901](https://github.com/advisories/GHSA-c9ph-gxww-7744): Sandboxed Thymeleaf expressions vulnerable to improper recognition of unauthorized syntax patterns

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf:3.1.3.RELEASE (declared at transitive dependency)
  - org.thymeleaf:thymeleaf-spring6:3.1.3.RELEASE (declared at transitive dependency)

Recommended fix:
  - Upgrade org.thymeleaf:thymeleaf to 3.1.5.RELEASE or later
  - Upgrade org.thymeleaf:thymeleaf-spring6 to 3.1.5.RELEASE or later

### CVE-2026-40478: Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-40478](https://github.com/advisories/GHSA-xjw8-8c5c-9r79): Improper neutralization of specific syntax patterns for unauthorized expressions in Thymeleaf

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf:3.1.3.RELEASE (declared at transitive dependency)
  - org.thymeleaf:thymeleaf-spring6:3.1.3.RELEASE (declared at transitive dependency)

Recommended fix:
  - Upgrade org.thymeleaf:thymeleaf to 3.1.4.RELEASE or later
  - Upgrade org.thymeleaf:thymeleaf-spring6 to 3.1.4.RELEASE or later

### CVE-2026-40477: Improper restriction of the scope of accessible objects in Thymeleaf expressions
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-40477](https://github.com/advisories/GHSA-r4v4-5mwr-2fwr): Improper restriction of the scope of accessible objects in Thymeleaf expressions

Severity: CRITICAL

Affected dependencies:
  - org.thymeleaf:thymeleaf:3.1.3.RELEASE (declared at transitive dependency)
  - org.thymeleaf:thymeleaf-spring6:3.1.3.RELEASE (declared at transitive dependency)

Recommended fix:
  - Upgrade org.thymeleaf:thymeleaf to 3.1.4.RELEASE or later
  - Upgrade org.thymeleaf:thymeleaf-spring6 to 3.1.4.RELEASE or later

### CVE-2024-47072: XStream is vulnerable to a Denial of Service attack due to stack overflow from a manipulated binary input stream
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2024-47072](https://github.com/advisories/GHSA-hfq9-hggm-c56q): XStream is vulnerable to a Denial of Service attack due to stack overflow from a manipulated binary input stream

Severity: HIGH

Affected dependencies:
  - com.thoughtworks.xstream:xstream:1.4.20 (declared at transitive dependency)

Recommended fix:
  - Upgrade com.thoughtworks.xstream:xstream to 1.4.21 or later

### CVE-2026-42587: Netty: HttpContentDecompressor maxAllocation bypass when Content-Encoding set to br/zstd/snappy leads to decompression bomb DoS
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-42587](https://github.com/advisories/GHSA-f6hv-jmp6-3vwv): Netty: HttpContentDecompressor maxAllocation bypass when Content-Encoding set to br/zstd/snappy leads to decompression bomb DoS

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http2 to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later
  - Upgrade io.netty:netty-codec-http2 to 4.1.133.Final or later

### CVE-2026-42584: Netty has HttpClientCodec response desynchronization
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-42584](https://github.com/advisories/GHSA-57rv-r2g8-2cj3): Netty has HttpClientCodec response desynchronization

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later

### CVE-2026-42583: Netty Lz4FrameDecoder is vulnerable to resource exhaustion 
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-42583](https://github.com/advisories/GHSA-mj4r-2hfc-f8p6): Netty Lz4FrameDecoder is vulnerable to resource exhaustion 

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec to 4.1.133.Final or later

### CVE-2026-42579: Netty has a DNS Codec Input Validation Bypass (Encoder + Decoder)
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-42579](https://github.com/advisories/GHSA-cm33-6792-r9fm): Netty has a DNS Codec Input Validation Bypass (Encoder + Decoder)

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-dns:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-dns:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-dns to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-dns to 4.1.133.Final or later

### CVE-2026-33871: Netty HTTP/2 CONTINUATION Frame Flood DoS via Zero-Byte Frame Bypass
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-33871](https://github.com/advisories/GHSA-w9fj-cfpg-grvv): Netty HTTP/2 CONTINUATION Frame Flood DoS via Zero-Byte Frame Bypass

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http2 to 4.1.132.Final or later
  - Upgrade io.netty:netty-codec-http2 to 4.2.11.Final or later

### CVE-2026-33870: Netty: HTTP Request Smuggling via Chunked Extension Quoted-String Parsing
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-33870](https://github.com/advisories/GHSA-pwqr-wmgm-9rr8): Netty: HTTP Request Smuggling via Chunked Extension Quoted-String Parsing

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.1.132.Final or later
  - Upgrade io.netty:netty-codec-http to 4.2.10.Final or later

### CVE-2025-55163: Netty affected by MadeYouReset HTTP/2 DDoS vulnerability
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-55163](https://github.com/advisories/GHSA-prj3-ccx8-p6x4): Netty affected by MadeYouReset HTTP/2 DDoS vulnerability

Severity: HIGH

Affected dependencies:
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http2:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http2 to 4.2.4.Final or later
  - Upgrade io.netty:netty-codec-http2 to 4.1.124.Final or later

### CVE-2025-24970: SslHandler doesn't correctly validate packets which can lead to native crash when using native SSLEngine
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-24970](https://github.com/advisories/GHSA-4g8c-wm8x-jfhw): SslHandler doesn't correctly validate packets which can lead to native crash when using native SSLEngine

Severity: HIGH

Affected dependencies:
  - io.netty:netty-handler:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-handler to 4.1.118.Final or later

### CVE-2026-41284: Apache Tomcat: Unbounded read in WebDAV LOCK and  PROPFIND handling
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-41284](https://github.com/advisories/GHSA-gx5v-xp9w-j4cg): Apache Tomcat: Unbounded read in WebDAV LOCK and  PROPFIND handling

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2026-43513: Apache Tomcat: LockOutRealm treats user names as case-sensitive
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-43513](https://github.com/advisories/GHSA-5mp6-jrq3-r938): Apache Tomcat: LockOutRealm treats user names as case-sensitive

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2026-42498: Apache Tomcat - WebSocket authentication header exposure
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-42498](https://github.com/advisories/GHSA-fv25-8xcx-gqjc): Apache Tomcat - WebSocket authentication header exposure

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.55 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.22 or later

### CVE-2026-5598: Bouncy Castle Has Covert Timing Channel Vulnerability
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-5598](https://github.com/advisories/GHSA-p93r-85wp-75v3): Bouncy Castle Has Covert Timing Channel Vulnerability

Severity: HIGH

Affected dependencies:
  - org.bouncycastle:bcprov-jdk18on:1.78.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.bouncycastle:bcprov-jdk18on to 1.84 or later

### CVE-2026-34483: Apache Tomcat has an Improper Encoding or Escaping of Output vulnerability in the JsonAccessLogValve
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-34483](https://github.com/advisories/GHSA-rv64-5gf8-9qq8): Apache Tomcat has an Improper Encoding or Escaping of Output vulnerability in the JsonAccessLogValve

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.54 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.21 or later

### CVE-2026-34487: Apache Tomcat vulnerable to Insertion of Sensitive Information into Log File
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-34487](https://github.com/advisories/GHSA-x4m4-345f-5h5g): Apache Tomcat vulnerable to Insertion of Sensitive Information into Log File

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.54 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.21 or later

### CVE-2026-24880: Apache Tomcat has an HTTP Request/Response Smuggling vulnerability
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-24880](https://github.com/advisories/GHSA-563x-q5rq-57qp): Apache Tomcat has an HTTP Request/Response Smuggling vulnerability

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.52 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.20 or later

### CVE-2026-24734: Apache Tomcat has an Improper Input Validation vulnerability
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-24734](https://github.com/advisories/GHSA-mgp5-rv84-w37q): Apache Tomcat has an Improper Input Validation vulnerability

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.18 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.52 or later

### CVE-2025-55752: Apache Tomcat Vulnerable to Relative Path Traversal
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-55752](https://github.com/advisories/GHSA-wmwf-9ccg-fff5): Apache Tomcat Vulnerable to Relative Path Traversal

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.11 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.45 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.109 or later

### CVE-2025-48989: Apache Tomcat Improper Resource Shutdown or Release vulnerability
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-48989](https://github.com/advisories/GHSA-gqp3-2cvr-x8m3): Apache Tomcat Improper Resource Shutdown or Release vulnerability

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.10 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.44 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.108 or later

### CVE-2025-53506: Apache Tomcat Coyote vulnerable to Denial of Service via excessive HTTP/2 streams
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-53506](https://github.com/advisories/GHSA-25xr-qj8w-c4vf): Apache Tomcat Coyote vulnerable to Denial of Service via excessive HTTP/2 streams

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.107 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.43 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.9 or later

### CVE-2025-52520: Apache Tomcat Catalina is vulnerable to DoS attack through bypassing of size limits
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-52520](https://github.com/advisories/GHSA-wr62-c79q-cv37): Apache Tomcat Catalina is vulnerable to DoS attack through bypassing of size limits

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.9 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.43 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.107 or later

### CVE-2025-48988: Apache Tomcat - DoS in multipart upload
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-48988](https://github.com/advisories/GHSA-h3gc-qfqq-6h8f): Apache Tomcat - DoS in multipart upload

Severity: HIGH

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.8 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.42 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.106 or later

### CVE-2025-27820: Apache HttpClient disables domain checks
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-27820](https://github.com/advisories/GHSA-73m2-qfq3-56cx): Apache HttpClient disables domain checks

Severity: HIGH

Affected dependencies:
  - org.apache.httpcomponents.client5:httpclient5:5.4.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.httpcomponents.client5:httpclient5 to 5.4.3 or later

### CVE-2026-40972: Spring Boot DevTools remote secret comparison is vulnerable to timing attacks
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-api-gateway/pom.xml:32

[CVE-2026-40972](https://github.com/advisories/GHSA-56v8-86gj-66jp): Spring Boot DevTools remote secret comparison is vulnerable to timing attacks

Severity: HIGH

Affected dependencies:
  - org.springframework.boot:spring-boot-devtools:3.4.1 (declared at spring-petclinic-api-gateway/pom.xml:32)

### CVE-2026-22733: Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-vets-service/pom.xml:33, spring-petclinic-visits-service/pom.xml:24

[CVE-2026-22733](https://github.com/advisories/GHSA-mgvc-8q2h-5pgc): Spring Boot has an Authentication Bypass under Actuator CloudFoundry endpoints

Severity: HIGH

Affected dependencies:
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-vets-service/pom.xml:33, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-visits-service/pom.xml:24)
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-vets-service/pom.xml:33, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-visits-service/pom.xml:24)

Recommended fix:
  - Upgrade org.springframework.boot:spring-boot-starter-actuator to 4.0.4 or later

### CVE-2026-22731: Spring Boot has an Authentication Bypass under Actuator Health groups paths
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-vets-service/pom.xml:33, spring-petclinic-visits-service/pom.xml:24

[CVE-2026-22731](https://github.com/advisories/GHSA-8hfc-fq58-r658): Spring Boot has an Authentication Bypass under Actuator Health groups paths

Severity: HIGH

Affected dependencies:
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-vets-service/pom.xml:33, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-visits-service/pom.xml:24)
  - org.springframework.boot:spring-boot-starter-actuator:3.4.1 (declared at spring-petclinic-vets-service/pom.xml:33, spring-petclinic-customers-service/pom.xml:25, spring-petclinic-api-gateway/pom.xml:42, spring-petclinic-genai-service/pom.xml:39, spring-petclinic-visits-service/pom.xml:24)

Recommended fix:
  - Upgrade org.springframework.boot:spring-boot-starter-actuator to 4.0.4 or later

### CVE-2026-41002: Spring Cloud Config Server Susceptible To TOCTOU Attack
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-config-server/pom.xml:31

[CVE-2026-41002](https://github.com/advisories/GHSA-86wq-234q-r6wg): Spring Cloud Config Server Susceptible To TOCTOU Attack

Severity: HIGH

Affected dependencies:
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:31)

### CVE-2026-40973: Spring Boot accepts predictable temp directory without ownership verification
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2026-40973](https://github.com/advisories/GHSA-wwpq-f5c3-7hvx): Spring Boot accepts predictable temp directory without ownership verification

Severity: HIGH

Affected dependencies:
  - org.springframework.boot:spring-boot:3.4.1 (declared at transitive dependency)

### CVE-2026-22739: Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** spring-petclinic-config-server/pom.xml:31

[CVE-2026-22739](https://github.com/advisories/GHSA-3qwq-q9vm-5j42): Spring Cloud Config Server: Path Traversal via Profile Parameter Allows Arbitrary File Access

Severity: HIGH

Affected dependencies:
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:31)
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:31)

Recommended fix:
  - Upgrade org.springframework.cloud:spring-cloud-config-server to 5.0.2 or later

### CVE-2025-41253: Spring Cloud Gateway Server Webflux is vulnerable to Expression Language Injection
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-41253](https://github.com/advisories/GHSA-fwxx-wv44-7qfg): Spring Cloud Gateway Server Webflux is vulnerable to Expression Language Injection

Severity: HIGH

Affected dependencies:
  - org.springframework.cloud:spring-cloud-gateway-server:4.2.0 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework.cloud:spring-cloud-gateway-server to 4.2.6 or later

### CVE-2025-41249: Spring Framework annotation detection mechanism may result in improper authorization
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-41249](https://github.com/advisories/GHSA-jmp9-x22r-554x): Spring Framework annotation detection mechanism may result in improper authorization

Severity: HIGH

Affected dependencies:
  - org.springframework:spring-core:6.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework:spring-core to 6.2.11 or later

### CVE-2025-41235: Spring Cloud Gateway Server Forwards Headers from Untrusted Proxies
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-41235](https://github.com/advisories/GHSA-6j2q-c73v-97c5): Spring Cloud Gateway Server Forwards Headers from Untrusted Proxies

Severity: HIGH

Affected dependencies:
  - org.springframework.cloud:spring-cloud-gateway-server:4.2.0 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework.cloud:spring-cloud-gateway-server to 4.2.3 or later

### CVE-2025-22235: Spring Boot EndpointRequest.to() creates wrong matcher if actuator endpoint is not exposed
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-22235](https://github.com/advisories/GHSA-rc42-6c7j-7h5r): Spring Boot EndpointRequest.to() creates wrong matcher if actuator endpoint is not exposed

Severity: HIGH

Affected dependencies:
  - org.springframework.boot:spring-boot:3.4.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework.boot:spring-boot to 3.4.5 or later

### CVE-2025-22228: Spring Security Does Not Enforce Password Length
- **Severity:** mandatory
- **Story Points:** 1

[CVE-2025-22228](https://github.com/advisories/GHSA-mg83-c7gq-rv5c): Spring Security Does Not Enforce Password Length

Severity: HIGH

Affected dependencies:
  - org.springframework.security:spring-security-crypto:6.4.2 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework.security:spring-security-crypto to 6.4.4 or later

### GHSA-72hv-8253-57qq: jackson-core: Number Length Constraint Bypass in Async Parser Leads to Potential DoS Condition
- **Severity:** optional
- **Story Points:** 1

[GHSA-72hv-8253-57qq](https://github.com/advisories/GHSA-72hv-8253-57qq): jackson-core: Number Length Constraint Bypass in Async Parser Leads to Potential DoS Condition

Severity: MEDIUM

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-core:2.18.2 (declared at transitive dependency)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-core to 2.18.6 or later

### CVE-2025-11226: QOS.CH logback-core is vulnerable to Arbitrary Code Execution through file processing
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-11226](https://github.com/advisories/GHSA-25qh-j22f-pwp8): QOS.CH logback-core is vulnerable to Arbitrary Code Execution through file processing

Severity: MEDIUM

Affected dependencies:
  - ch.qos.logback:logback-core:1.5.12 (declared at transitive dependency)

Recommended fix:
  - Upgrade ch.qos.logback:logback-core to 1.5.19 or later

### CVE-2024-12798: QOS.CH logback-core Expression Language Injection vulnerability
- **Severity:** optional
- **Story Points:** 1

[CVE-2024-12798](https://github.com/advisories/GHSA-pr98-23f8-jwxv): QOS.CH logback-core Expression Language Injection vulnerability

Severity: MEDIUM

Affected dependencies:
  - ch.qos.logback:logback-core:1.5.12 (declared at transitive dependency)

Recommended fix:
  - Upgrade ch.qos.logback:logback-core to 1.5.13 or later

### CVE-2025-48924: Apache Commons Lang is vulnerable to Uncontrolled Recursion when processing long inputs
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-48924](https://github.com/advisories/GHSA-j288-q9x7-2f5v): Apache Commons Lang is vulnerable to Uncontrolled Recursion when processing long inputs

Severity: MEDIUM

Affected dependencies:
  - org.apache.commons:commons-lang3:3.17.0 (declared at transitive dependency)
  - commons-lang:commons-lang:2.6 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.commons:commons-lang3 to 3.18.0 or later

### CVE-2026-42585: Netty vulnerable to HTTP Request Smuggling due to malformed Transfer-Encoding
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-42585](https://github.com/advisories/GHSA-38f8-5428-x5cv): Netty vulnerable to HTTP Request Smuggling due to malformed Transfer-Encoding

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later

### CVE-2026-42581: Netty HTTP/1.0 TE+CL Coexistence Bypasses Smuggling Sanitization
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-42581](https://github.com/advisories/GHSA-xxqh-mfjm-7mv9): Netty HTTP/1.0 TE+CL Coexistence Bypasses Smuggling Sanitization

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later

### CVE-2026-42580: Netty vulnerable to HTTP Request Smuggling due to incorrect chunk size parsing
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-42580](https://github.com/advisories/GHSA-m4cv-j2px-7723): Netty vulnerable to HTTP Request Smuggling due to incorrect chunk size parsing

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later

### CVE-2026-41417: Netty: Start-Line Injection in DefaultHttpRequest.setUri() Allows HTTP Request Smuggling and RTSP Request Injection
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-41417](https://github.com/advisories/GHSA-v8h7-rr48-vmmv): Netty: Start-Line Injection in DefaultHttpRequest.setUri() Allows HTTP Request Smuggling and RTSP Request Injection

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.1.133.Final or later
  - Upgrade io.netty:netty-codec-http to 4.2.13.Final or later

### CVE-2025-67735: Netty has a CRLF Injection vulnerability in io.netty.handler.codec.http.HttpRequestEncoder
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-67735](https://github.com/advisories/GHSA-84h7-rjj3-6jx4): Netty has a CRLF Injection vulnerability in io.netty.handler.codec.http.HttpRequestEncoder

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)
  - io.netty:netty-codec-http:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec-http to 4.2.8.Final or later
  - Upgrade io.netty:netty-codec-http to 4.1.129.Final or later

### CVE-2025-58057: Netty's decoders vulnerable to DoS via zip bomb style attack
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-58057](https://github.com/advisories/GHSA-3p8m-j85q-pgmj): Netty's decoders vulnerable to DoS via zip bomb style attack

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-codec:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-codec to 4.1.125.Final or later

### CVE-2025-25193: Denial of Service attack on windows app using Netty
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-25193](https://github.com/advisories/GHSA-389x-839f-4rhx): Denial of Service attack on windows app using Netty

Severity: MEDIUM

Affected dependencies:
  - io.netty:netty-common:4.1.116.Final (declared at transitive dependency)

Recommended fix:
  - Upgrade io.netty:netty-common to 4.1.118.Final or later

### CVE-2026-45292: OpenTelemetry Java SDK has Unbounded Memory Allocation in W3C Baggage Propagation
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-45292](https://github.com/advisories/GHSA-rcgg-9c38-7xpx): OpenTelemetry Java SDK has Unbounded Memory Allocation in W3C Baggage Propagation

Severity: MEDIUM

Affected dependencies:
  - io.opentelemetry:opentelemetry-api:1.43.0 (declared at transitive dependency)

Recommended fix:
  - Upgrade io.opentelemetry:opentelemetry-api to 1.62.0 or later

### CVE-2025-22227: Reactor Netty HTTP is vulnerable to credential leaks during chained redirects
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-22227](https://github.com/advisories/GHSA-4q2v-9p7v-3v22): Reactor Netty HTTP is vulnerable to credential leaks during chained redirects

Severity: MEDIUM

Affected dependencies:
  - io.projectreactor.netty:reactor-netty-http:1.2.1 (declared at transitive dependency)
  - io.projectreactor.netty:reactor-netty-http:1.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade io.projectreactor.netty:reactor-netty-http to 1.3.0-M5 or later
  - Upgrade io.projectreactor.netty:reactor-netty-http to 1.2.8 or later

### CVE-2020-36843: Ed25519 Signature Malleability in ed25519-java Due to Missing Scalar Range Check
- **Severity:** optional
- **Story Points:** 1

[CVE-2020-36843](https://github.com/advisories/GHSA-p53j-g8pw-4w5f): Ed25519 Signature Malleability in ed25519-java Due to Missing Scalar Range Check

Severity: MEDIUM

Affected dependencies:
  - net.i2p.crypto:eddsa:0.3.0 (declared at transitive dependency)

### CVE-2026-0636: Bouncy Castle has an LDAP injection
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-0636](https://github.com/advisories/GHSA-c3fc-8qff-9hwx): Bouncy Castle has an LDAP injection

Severity: MEDIUM

Affected dependencies:
  - org.bouncycastle:bcprov-jdk18on:1.78.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.bouncycastle:bcprov-jdk18on to 1.84 or later

### CVE-2026-25854: Apache Tomcat has an Open Redirect vulnerability
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-25854](https://github.com/advisories/GHSA-9m3c-qcxr-9x87): Apache Tomcat has an Open Redirect vulnerability

Severity: MEDIUM

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.53 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.20 or later

### CVE-2025-66614: Apache Tomcat - Client certificate verification bypass
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-66614](https://github.com/advisories/GHSA-fpj8-gq4v-p354): Apache Tomcat - Client certificate verification bypass

Severity: MEDIUM

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.15 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.50 or later

### CVE-2025-49124: Apache Tomcat installer for Windows has an untrusted search path vulnerability
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-49124](https://github.com/advisories/GHSA-42wg-hm62-jcwg): Apache Tomcat installer for Windows has an untrusted search path vulnerability

Severity: MEDIUM

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.8 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.42 or later

### CVE-2025-49125: Apache Tomcat - Security constraint bypass for pre/post-resources
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-49125](https://github.com/advisories/GHSA-wc4r-xq3c-5cf3): Apache Tomcat - Security constraint bypass for pre/post-resources

Severity: MEDIUM

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.8 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.42 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 9.0.106 or later

### CVE-2025-31650: Apache Tomcat Denial of Service via invalid HTTP priority header
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-31650](https://github.com/advisories/GHSA-3p2h-wqq4-wf4h): Apache Tomcat Denial of Service via invalid HTTP priority header

Severity: MEDIUM

Affected dependencies:
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)
  - org.apache.tomcat.embed:tomcat-embed-core:10.1.34 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 10.1.40 or later
  - Upgrade org.apache.tomcat.embed:tomcat-embed-core to 11.0.6 or later

### CVE-2020-13956: Cross-site scripting in Apache HttpClient
- **Severity:** optional
- **Story Points:** 1

[CVE-2020-13956](https://github.com/advisories/GHSA-7r82-7xv7-xcpj): Cross-site scripting in Apache HttpClient

Severity: MEDIUM

Affected dependencies:
  - org.apache.httpcomponents:httpclient:4.5.3 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.apache.httpcomponents:httpclient to 4.5.13 or later

### CVE-2025-4949: Eclipse JGit XML External Entity (XXE) Vulnerability
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-4949](https://github.com/advisories/GHSA-vrpq-qp53-qv56): Eclipse JGit XML External Entity (XXE) Vulnerability

Severity: MEDIUM

Affected dependencies:
  - org.eclipse.jgit:org.eclipse.jgit:6.10.0.202406032230-r (declared at transitive dependency)
  - org.eclipse.jgit:org.eclipse.jgit:6.10.0.202406032230-r (declared at transitive dependency)

Recommended fix:
  - Upgrade org.eclipse.jgit:org.eclipse.jgit to 6.10.1.202505221210-r or later
  - Upgrade org.eclipse.jgit:org.eclipse.jgit to 6.0.0.202111291000-r or later

### CVE-2026-41004: Spring Cloud Config Server Logged Sensitive Information
- **Severity:** optional
- **Story Points:** 1
- **Files:** spring-petclinic-config-server/pom.xml:31

[CVE-2026-41004](https://github.com/advisories/GHSA-j6hh-h3cf-c2hf): Spring Cloud Config Server Logged Sensitive Information

Severity: MEDIUM

Affected dependencies:
  - org.springframework.cloud:spring-cloud-config-server:4.2.0 (declared at spring-petclinic-config-server/pom.xml:31)

### CVE-2026-22745: Spring MVC and WebFlux applications are vulnerable to Denial of Service attacks when resolving static resources
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-22745](https://github.com/advisories/GHSA-6p4f-wcwh-5vvm): Spring MVC and WebFlux applications are vulnerable to Denial of Service attacks when resolving static resources

Severity: MEDIUM

Affected dependencies:
  - org.springframework:spring-webflux:6.2.1 (declared at transitive dependency)
  - org.springframework:spring-webmvc:6.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework:spring-webflux to 6.2.18 or later
  - Upgrade org.springframework:spring-webmvc to 6.2.18 or later

### CVE-2026-22737: Spring Framework Improper Path Limitation with Script View Templates
- **Severity:** optional
- **Story Points:** 1

[CVE-2026-22737](https://github.com/advisories/GHSA-4773-3jfm-qmx3): Spring Framework Improper Path Limitation with Script View Templates

Severity: MEDIUM

Affected dependencies:
  - org.springframework:spring-webmvc:6.2.1 (declared at transitive dependency)
  - org.springframework:spring-webmvc:6.2.1 (declared at transitive dependency)
  - org.springframework:spring-webflux:6.2.1 (declared at transitive dependency)
  - org.springframework:spring-webflux:6.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework:spring-webmvc to 7.0.6 or later
  - Upgrade org.springframework:spring-webmvc to 6.2.17 or later
  - Upgrade org.springframework:spring-webflux to 7.0.6 or later
  - Upgrade org.springframework:spring-webflux to 6.2.17 or later

### CVE-2025-41242: Spring Framework MVC Applications Path Traversal Vulnerability
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-41242](https://github.com/advisories/GHSA-r936-gwx5-v52f): Spring Framework MVC Applications Path Traversal Vulnerability

Severity: MEDIUM

Affected dependencies:
  - org.springframework:spring-webmvc:6.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework:spring-webmvc to 6.2.10 or later

### CVE-2025-41234: Spring Framework vulnerable to a reflected file download (RFD)
- **Severity:** optional
- **Story Points:** 1

[CVE-2025-41234](https://github.com/advisories/GHSA-6r3c-xf4w-jxjm): Spring Framework vulnerable to a reflected file download (RFD)

Severity: MEDIUM

Affected dependencies:
  - org.springframework:spring-web:6.2.1 (declared at transitive dependency)

Recommended fix:
  - Upgrade org.springframework:spring-web to 6.2.8 or later

## CWE Findings (Code-Level Vulnerabilities)

### CWE-567: Unsynchronized Access to Shared Data in a Multithreaded Context
- **Category:** Concurrency & Synchronization
- **Severity:** potential
- **Story Points:** 5
- **Files:** spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java

VisitsServiceClient is a Spring @Component singleton (lines 30-31). It stores mutable shared state in the instance field 'hostname' (line 34), reads it from getVisitsForPets() (lines 42-47), and writes it through setHostname() (lines 54-55) without any synchronization, volatile qualifier, or immutable design. In a multithreaded Spring request-processing context, concurrent reads/writes of this shared field can observe stale or inconsistent values.

### CWE-662: Improper Synchronization
- **Category:** Concurrency & Synchronization
- **Severity:** potential
- **Story Points:** 8
- **Files:** spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java

The singleton VisitsServiceClient bean exposes unsynchronized access to the shared 'hostname' field: request-handling threads use the field in getVisitsForPets() (lines 42-47) while setHostname() can modify it (lines 54-55). Because the shared resource is accessed from a singleton component without any synchronization mechanism, the code matches an improper synchronization pattern in concurrent execution.

### CWE-820: Missing Synchronization
- **Category:** Concurrency & Synchronization
- **Severity:** potential
- **Story Points:** 8
- **Files:** spring-petclinic-api-gateway/src/main/java/org/springframework/samples/petclinic/api/application/VisitsServiceClient.java

VisitsServiceClient keeps mutable shared state in the 'hostname' field (line 34) inside a Spring singleton bean (lines 30-31). The field is accessed by getVisitsForPets() and mutated by setHostname() with no synchronized block, lock, volatile declaration, or thread-safe wrapper. This is a direct missing-synchronization pattern for shared concurrent state.

### CWE-798: Use of Hard-coded Credentials
- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** spring-petclinic-genai-service/src/main/resources/application.yml

spring-petclinic-genai-service/src/main/resources/application.yml line 25 sets spring.ai.openai.api-key to ${OPENAI_API_KEY:demo}. The hard-coded fallback value 'demo' means the service will use an embedded credential when the environment variable is absent, which is a hard-coded outbound credential pattern.

### CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')
- **Category:** Injection Attacks
- **Severity:** optional
- **Story Points:** 8
- **Files:** spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/PetclinicChatClient.java

PetclinicChatClient.exchange() accepts arbitrary user-controlled request body content in the query parameter and returns chatClient.prompt().user(u -> u.text(query)).call().content() directly to the HTTP response without any output encoding or sanitization (lines 57-69). Because attacker-influenced content is reflected back as raw response text, this matches the XSS pattern of unescaped user input in responses.

### CWE-99: Improper Control of Resource Identifiers ('Resource Injection')
- **Category:** Injection Attacks
- **Severity:** potential
- **Story Points:** 3
- **Files:** spring-petclinic-genai-service/src/main/java/org/springframework/samples/petclinic/genai/AIDataProvider.java

AIDataProvider.addPetToOwner() builds a downstream resource URI by concatenating request.ownerId() into ownersHostname + "owners/" + request.ownerId() + "/pets" (line 64). The ownerId value originates from the AddPetRequest input supplied through the AI-exposed function interface, so externally influenced input is used directly as a resource identifier for an internal HTTP resource without server-side restriction.
