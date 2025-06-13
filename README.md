# mygene-v2-platform

## 2. `mygene-v2-platform` (Core Backend)

```markdown
# myGENE v2 - The Ubiquitous Digital Layer

**Status:** `Active Development` | **Version:** 2.1.0 | **License:** MIT

Welcome to the future of myGENE! This repository represents the evolution of our platform into a ubiquitous, API-first digital agency layer. This is the core backend platform that powers all user-facing applications, extensions, and plugins.

### Architectural Overview

myGENE v2 is built on a scalable, secure, and distributed microservices architecture.

* **Architecture Style:** API-First, Microservices
* **Backend:** Node.js, Python, and Go microservices running in Docker containers, orchestrated by Kubernetes.
* **Key Services:**
    * `identity-service`: Manages DIDs and Verifiable Credentials (ZKP logic).
    * `ai-service`: Handles all interactions with LLMs (Gemini), including briefings, greetings, and NLP tasks.
    * `task-service`: Executes autonomous actions for the user.
    * `dashboard-api`: The core API gateway for all myGENE dashboard interactions.
* **Database:** Polyglot persistence (PostgreSQL for relational data, MongoDB for logs and unstructured data).
* **Deployment:** Multi-region deployment on Google Cloud Platform (GCP).

### Key Features (v2)
* Decentralized Identity (DID) and Zero-Knowledge Proof verification.
* Full API for all myGENE Dashboard and plugin functionality.
* SDKs for Browser Extension and Third-Party Plugin development.
* Advanced AI-powered proactive assistance and personalization.
* Powers both the Citizen and Governance Dashboards.

### Setup & Installation
> Detailed setup instructions for individual microservices can be found in their respective subdirectories. A Docker Compose file is provided for local development environments.
```bash
# Clone the repository
git clone [https://github.com/mygene-project/mygene-v2-platform.git](https://github.com/mygene-project/mygene-v2-platform.git)
cd mygene-v2-platform

# Bring up the local environment
docker-compose up -d
