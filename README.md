## Hi, I'm Harshith 👋

**Software Engineer: DevOps Tooling, Cloud & AI** · MSc Data Science, Middlesex University · UK

I build well-tested services and the tooling that ships them: Python and
FastAPI, Docker and Kubernetes, GitHub Actions pipelines with security gates,
and data pipelines with DuckDB and scikit-learn. I also build AI-powered DevOps
tools with LLMs such as Claude (Anthropic) and OpenAI GPT models. I'm looking for a graduate
**Software Engineer / DevOps** role in the UK.

### Featured projects

**[Agentic Data Analyst](https://github.com/harshithkonatham/agentic-data-analyst)**: a team of Claude agents that analyses any CSV like a data team

- **Planner → Analyst → Reviewer** agents built on the Anthropic SDK (tool runner + structured outputs)
- Every number comes from a real tool (pandas, scikit-learn); every finding must cite the tool call behind it, and the Reviewer flags overclaims before they reach the report
- Offline mode runs the same tools without an API key; 20 tests, ~97% coverage, CI with security scans

**[Edge IoT Anomaly Agent](https://github.com/harshithkonatham/edge-iot-anomaly-agent)**: predictive maintenance for industrial motors (combines my ECE degree with data science)

- Streaming detector (robust z-score + stuck-sensor check) small enough for an edge gateway; sensor history in **DuckDB**
- A Claude agent investigates each incident with SQL tools, fleet comparison and maintenance runbooks, and returns a schema-validated diagnosis
- Simulated fleet with injected faults gives ground truth: 100% recall and precision on the baseline scenarios, scored in CI

**[Secure Payments API](https://github.com/harshithkonatham/devops-ai-toolkit/tree/main/projects/payments-api)**: a card-transactions service built to show a secure SDLC end to end

- Card numbers are never stored or logged (last 4 digits + HMAC fingerprint); JWT auth with per-user authorisation; idempotent payments
- Transactional outbox → **RabbitMQ** → risk-monitor consumer, with idempotent processing and a dead-letter queue
- CI gates: pytest (≥90% coverage), Semgrep, Bandit, CodeQL, Gitleaks, pip-audit, Checkov, Grype + SBOM, then deploy to Kubernetes and run end-to-end tests
- **Terraform** for AWS (KMS, ECR, CloudWatch, Secrets Manager, GitHub OIDC), Prometheus alerts with unit tests, a Grafana dashboard, runbooks, and a **PCI DSS v4.0** control mapping

**[AI DevOps Agents](https://github.com/harshithkonatham/devops-ai-toolkit/tree/main/tools/ai-agents)**: LLM-powered tools that take repetitive work off DevOps teams

- AI pull-request reviewer that runs in **GitHub Actions** and uses the **Claude API** (Anthropic SDK)
- Incident responder that triages alerts and drafts runbooks; a **CrewAI** team of DevOps agents
- [LLM-Ops model benchmark](https://github.com/harshithkonatham/devops-ai-toolkit/tree/main/tools/llm-ops) that compares models on quality, speed and cost per call

**[Flight Delay Prediction](https://github.com/harshithkonatham/flight-delay-prediction)**: my MSc dissertation, rebuilt as a data pipeline and prediction API

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
| AI & LLMs | Claude API (Anthropic SDK: tool use, structured outputs, multi-agent workflows), OpenAI API (GPT models), CrewAI, LangChain, LiteLLM, Ollama |
| AI-assisted development | Claude Code, GitHub Copilot |

### Education

- **MSc Data Science with Integrated Placement**, Middlesex University, London (Jan 2025 – present): Machine Learning Foundations, Applied Data Analytics, Big Data Systems, Cloud Architecture. Thesis: *Cloud-Native ML Platform Engineering on Kubernetes*
- **BTech Electronics & Communication**, Sir C R Reddy College of Engineering, India (2020 – 2024): First Class Honours; elected President of the IETE Student Chapter

### Certifications

AWS Cloud Foundations (Eduskills) · Pega CSA / CSSA (trainee)
