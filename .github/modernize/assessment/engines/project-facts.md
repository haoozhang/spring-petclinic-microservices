# Project Facts

## Container Engine

| Field | Value |
|-------|-------|
| **Status** | ✅ success |
| **Confidence** | High |
| **Finding** | Docker is the primary container engine used, with Podman also explicitly supported as an alternative. Docker Compose is used for local multi-service orchestration. Images are built via a multi-stage Dockerfile using the Maven buildDocker profile with docker buildx for multi-platform support. |

**Values:**
- Docker (primary)
- Podman (supported alternative)
- Docker Compose v2 (local orchestration)
- docker buildx (multi-platform builds: linux/amd64, linux/arm64)

**Evidence:**
- `docker/Dockerfile` — multi-stage Dockerfile using eclipse-temurin:17 base image
- `docker-compose.yml` — Docker Compose file orchestrating all 9 services
- `pom.xml` — `<container.executable>docker</container.executable>` with note that podman is also supported
- `README.md` — documents both `docker compose up` and `podman-compose up` as startup options
- `README.md` — documents `-Dcontainer.executable=podman` override for Podman builds
- Maven buildDocker profile uses exec-maven-plugin to invoke the container executable with docker buildx --platform flags

---

## Base Image

| Field | Value |
|-------|-------|
| **Status** | ✅ success |
| **Confidence** | High |
| **Finding** | The application services use eclipse-temurin:17 as the base image in a multi-stage Dockerfile. The build stage and final runtime stage both use eclipse-temurin:17 (Eclipse Temurin JDK/JRE 17 from Adoptium). Supporting infrastructure images use grafana/grafana:5.2.4 and prom/prometheus:v2.4.2. |

**Values:**
- `eclipse-temurin:17` (application services — build and runtime stages)
- `grafana/grafana:5.2.4` (monitoring)
- `prom/prometheus:v2.4.2` (metrics)
- Ubuntu-based (Eclipse Temurin 17 is built on Ubuntu)
- Docker Hub registry (all images)

**Evidence:**
- `docker/Dockerfile` line 1: `FROM eclipse-temurin:17 AS builder` (build stage)
- `docker/Dockerfile` line 8: `FROM eclipse-temurin:17` (final runtime stage)
- `docker/grafana/Dockerfile` line 1: `FROM grafana/grafana:5.2.4`
- `docker/prometheus/Dockerfile` line 1: `FROM prom/prometheus:v2.4.2`
- Multi-stage build pattern used for application services (builder + runtime stages)
