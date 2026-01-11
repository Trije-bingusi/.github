# RSO project — UL FRI

Organization for a course project at the University of Ljubljana, Faculty of Computer and Information Science (UL FRI).  
The project is developed by three students (Janez Tomšič, Matija Bažec, Matic Zadobovšek) and represents a finished microservices-based learning platform.

---

## Platform overview

The platform (eUčilnica+) supports the full study workflow:

- **Courses & lectures**  
  Professors can create courses and add lectures with video recordings.

- **Lecture view**  
  Each lecture has a dedicated page with:
  - video playback,
  - automatically generated **transcription (subtitles)**,
  - **AI-generated summary**,
  - personal **student notes**,
  - course-level **forum discussions**.

- **Forum**  
  Each course includes a forum for creating threads and posts, implemented as a serverless service.

- **Authentication & roles**  
  Users authenticate via **Keycloak (OIDC)**.  
  Roles (student / professor) control access to write operations.

- **Architecture**  
  - REST APIs exposed through a **single API Gateway**
  - Deployed to **Azure Kubernetes Service (AKS)**
  - TLS via **NGINX Ingress + cert-manager + Let’s Encrypt**
  - Monitoring with Prometheus & Grafana
  - Centralized Logging with Promtail & Loki

---

## Repositories

### Application services
- **svc-courses** – Courses & lectures service
- **svc-users** – User profile service
- **svc-notes** – Personal notes service
- **svc-video** – Video management service
- **svc-transcription** – Lecture video transcription service
- **svc-summary** – AI-based text summarization service
- **svc-forum** – Serverless forum service

### Platform & infrastructure
- **svc-gateway** – API Gateway (routing, auth, RBAC, metrics)
- **rso-frontend** – Web frontend (Nuxt / Vue.js)
- **shared-infrastructure** – Terraform definitions for AKS, ACR, Key Vault, Ingress, Keycloak...
- **rso-platform** – Local integration and testing setup (Docker Compose)

Each repository has its own README with setup instructions, local development steps, and deployment details.

---

## Contributing

This repository group represents a **course project**.  
External contributions are **not accepted**; pull requests from non-members will be closed.

---

© UL FRI — RSO course project
