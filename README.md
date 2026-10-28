## Hi, I'm Harshith 👋

**Software Engineer: DevSecOps, Cloud & Data** · MSc Data Science, Middlesex University · UK

I build secure, well-tested services and the pipelines that ship them: Python
and FastAPI, Docker and Kubernetes, GitHub Actions with security gates, and
data pipelines with DuckDB and scikit-learn. I'm looking for a graduate
**Software Engineer / DevSecOps** role in the UK.

### Featured projects

**[Secure Payments API](https://github.com/harshithkonatham/dev-toolkit/tree/main/projects/payments-api)**: a card-transactions service built to show a secure SDLC end to end

- Card numbers are never stored or logged (last 4 digits + HMAC fingerprint); JWT auth with per-user authorisation; idempotent payments
- Transactional outbox → **RabbitMQ** → risk-monitor consumer, with idempotent processing and a dead-letter queue
- CI gates: pytest (≥90% coverage), Semgrep, Bandit, CodeQL, Gitleaks, pip-audit, Checkov, Grype + SBOM, then deploy to Kubernetes and run end-to-end tests
- **Terraform** for AWS (KMS, ECR, CloudWatch, Secrets Manager, GitHub OIDC), Prometheus alerts with unit tests, a Grafana dashboard, runbooks, and a **PCI DSS v4.0** control mapping

**[Flight Delay Prediction](https://github.com/harshithkonatham/prediction-for-airline-flight-delays)**: my MSc dissertation, rebuilt as a data pipeline and prediction API

- Ingests **2.2 M US flights** from public BTS data into Parquet with DuckDB, with 14 data-quality checks
- Found and fixed target leakage in the original notebook (100% "accuracy" → an honest ROC-AUC of 0.65 on unseen later dates)
- FastAPI prediction service in a hardened container; CI with security scans and a container smoke test

### Tech

| Area | Tools |
|---|---|
| Languages | Python, SQL, Java, JavaScript |
| Backend & messaging | FastAPI, REST APIs, RabbitMQ, SQLite / MySQL |
| CI/CD & DevSecOps | GitHub Actions, Docker, Kubernetes, Semgrep, Bandit, CodeQL, Gitleaks, pip-audit, Grype, Checkov, SBOM |
| Cloud & IaC | AWS (EC2, S3, IAM, VPC, CloudWatch, KMS, ECR), Terraform |
| Observability | Prometheus, Grafana, structured logging |
| Data & ML | Pandas, NumPy, DuckDB, Parquet, scikit-learn, Matplotlib |
| Testing & quality | pytest (unit, integration, e2e), mypy, Ruff |
| AI-assisted development | Claude Code, GitHub Copilot |

### Certifications

AWS Cloud Foundations (Eduskills) · Pega CSA / CSSA (trainee)
