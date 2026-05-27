# Security Assessment Report

**Generated:** 2026-05-27T02:31:31.762563Z

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 1 |
| CVE Vulnerabilities | 0 |
| CWE Vulnerabilities | 1 |
| Total Rules Assessed | 59 |
| Rules Passed | 58 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 0 |
| optional | 1 |
| potential | 0 |

## CVE Findings (Dependency Vulnerabilities)

No CVE findings at the configured threshold (critical).

## CWE Findings (Code-Level Vulnerabilities)

### CWE-798: Use of Hard-coded Credentials
- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** spring-petclinic-genai-service/src/main/resources/application.yml:25

Configuration contains a default credential value in `api-key: ${OPENAI_API_KEY:demo}` within the main application profile, which constitutes a hard-coded credential fallback.

