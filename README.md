## Hi, I'm Harshith 👋

**Software Engineer: DevOps Tooling, Cloud & AI** · MSc Data Science, Middlesex University · UK

I build well-tested services and the tooling that ships them: Python and
FastAPI, Docker and Kubernetes, GitHub Actions pipelines with security gates,
and data pipelines with DuckDB and scikit-learn. I also build AI-powered DevOps
tools with LLMs such as Claude (Anthropic) and OpenAI GPT models. I'm looking for a graduate
**Software Engineer / DevOps** role in the UK.

### Featured projects

**[Secure Payments API](https://github.com/harshithkonatham/dev-toolkit/tree/main/projects/payments-api)**: a card-transactions service built to show a secure SDLC end to end

- Card numbers are never stored or logged (last 4 digits + HMAC fingerprint); JWT auth with per-user authorisation; idempotent payments
- Transactional outbox → **RabbitMQ** → risk-monitor consumer, with idempotent processing and a dead-letter queue
- CI gates: pytest (≥90% coverage), Semgrep, Bandit, CodeQL, Gitleaks, pip-audit, Checkov, Grype + SBOM, then deploy to Kubernetes and run end-to-end tests
- **Terraform** for AWS (KMS, ECR, CloudWatch, Secrets Manager, GitHub OIDC), Prometheus alerts with unit tests, a Grafana dashboard, runbooks, and a **PCI DSS v4.0** control mapping

**[AI DevOps Agents](https://github.com/harshithkonatham/dev-toolkit/tree/main/tools/ai-agents)**: LLM-powered tools that take repetitive work off DevOps teams

- AI pull-request reviewer that runs in **GitHub Actions** and uses the **Claude API** (Anthropic SDK)
- Incident responder that triages alerts and drafts runbooks; a **CrewAI** team of DevOps agents
- [LLM-Ops model benchmark](https://github.com/harshithkonatham/dev-toolkit/tree/main/tools/llm-ops) that compares models on quality, speed and cost per call

**[Flight Delay Prediction](https://github.com/harshithkonatham/prediction-for-airline-flight-delays)**: my MSc dissertation, rebuilt as a data pipeline and prediction API

- Ingests **2.2 M US flights** from public BTS data into Parquet with DuckDB, with 14 data-quality checks
- Found and fixed target leakage in the original notebook (100% "accuracy" → an honest ROC-AUC of 0.65 on unseen later dates)
- FastAPI prediction service in a hardened container; CI with security scans and a container smoke test

### Tech

| Area | Tools |
|---|---|
| Languages | Python, SQL, Java, JavaScript |
| Backend & messaging | FastAPI, REST APIs, RabbitMQ, SQLite / MySQL |
| CI/CD & DevOps tooling | GitHub Actions, Docker, Kubernetes, Semgrep, Bandit, CodeQL, Gitleaks, pip-audit, Grype, Checkov, SBOM |
| Cloud & IaC | AWS (EC2, S3, IAM, VPC, CloudWatch, KMS, ECR), Terraform |
| Observability | Prometheus, Grafana, structured logging |
| Data & ML | Pandas, NumPy, DuckDB, Parquet, scikit-learn, Matplotlib |
| Testing & quality | pytest (unit, integration, e2e), mypy, Ruff |
| AI & LLMs | Claude API (Anthropic SDK), OpenAI API (GPT models), CrewAI, LangChain, LiteLLM, Ollama |
| AI-assisted development | Claude Code, GitHub Copilot |

### Certifications

AWS Cloud Foundations (Eduskills) · Pega CSA / CSSA (trainee)
