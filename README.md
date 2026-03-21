# 👋 Hey there, I’m Steven Horton

**Security Engineer | 16 years across fintech, e-commerce, and AI**

Security engineer who treats clarity as the first line of defense. I obsess over making the vulnerable path impossible to take by accident.

- 🔍 Built observability that made a crypto exchange breach immediately visible — contained it with zero customer impact.
- 🛠️ Author of security tooling that catches what scanners, frameworks, and best practices miss.
- 🤖 Built real-time fraud-detection that blocked 52%+ of bot traffic, safeguarding millions in annual marketing spend.

---

## 🚀 Featured Projects

### 🥒 [Pickle](https://github.com/shortontech/pickle) — The World’s Most Secure Web Framework

A code generation framework for **Go** that makes entire vulnerability classes structurally impossible. You write controllers, migrations, request classes, and middleware. Pickle generates plain, idiomatic Go. The output compiles to a single static binary with no runtime dependency on Pickle.

**Impossible by construction:**
- **SQL injection** — parameterized queries exclusively. No API for string interpolation. The unsafe path doesn’t exist.
- **Mass assignment** — request structs define exactly which fields are accepted. Unvalidated input never reaches the model.
- **IDOR** — `pickle squeeze` traces route → middleware → controller → query and verifies the chain is scoped by owner. No other framework does this.
- **Data tampering** — immutable tables are cryptographically hash-chained with SHA-256. Merkle tree checkpoints give O(log n) inclusion proofs you can hand to an auditor.

**Built for AI:** A functioning Pickle app is ~2,000 tokens of source. Ships an MCP server that gives AI models queryable access to your project’s structure — routes, middleware, validation rules, schema — without dumping source files into context.

---

### 🦅 [TelHawk Stack](https://github.com/telhawk-systems/telhawk-stack) — Open Cybersecurity SIEM Platform

An **OCSF-compliant**, **Go-based** SIEM platform using **OpenSearch** for log storage and analysis. Built on the principle of high-context UI design to optimize for AI and human efficiency.

- Modular microservices for **auth**, **ingestion**, **query**, and **visualization**.
- CLI tool (`thawk`) for token management, event ingestion, and SPL-style searches.
- Splunk HEC-compatible ingestion for easy migration from proprietary platforms.

---

## 🧠 Tech Arsenal

`Go` • `Python` • `TypeScript` • `SQL` • `C#` • `Docker` • `Kubernetes` • `AWS` • `Terraform` • `PostgreSQL` • `Kafka` • `GitHub Actions` • `GitLab`

---

## 💼 Career Highlights

### Horton Security Consulting — Independent Consultant (Apr 2025 – Present)
Incident response and infrastructure hardening across multiple client organizations. Built static analysis tooling in Go using tree-sitter that performs deterministic security analysis across Django, Laravel, and Rails codebases — identified a vulnerability in a major open-source project within five hours, resulting in an invitation to their private bug bounty program.

---

### Bitcoin Solutions — Security Engineering Lead (Aug 2022 – Apr 2025)
Rebuilt logging infrastructure and layered real-time analytics on top, catching a breach that would have been invisible under the previous setup. Red-teamed OpenAI and Anthropic models for customer support automation — built reproducible jailbreak exploits via prompt injection and narrative manipulation, recommended against deployment. Enforced automated security scanning (SAST/DAST/dependencies) in GitLab pipelines without exceptions.

---

### SDK Worldwide LLC — Security & Data Engineer (Feb 2019 – Apr 2022)
Built secure ETL pipelines in Python unifying data from Google Ads, Facebook, Stripe, and PayPal. Designed real-time anomaly detection that caught ad fraud before it drained customer budgets, blocking 52% of bot traffic. Managed security operations across client organizations — removed backdoors, revoked orphaned access, unified access controls via OAuth and secrets management.

---

### Capital Research International — Security Engineering Lead (Mar 2017 – Sep 2018)
Set standards for four developers: code reviews, automated testing, CI/CD with feature flags. Daily releases, zero rollback. Defended against persistent APT-level threats (China, North Korea) with zero breaches using honeypots to misdirect attackers into controlled environments. Consolidated 15 fragmented systems into a single API surface.

---

### MAS Group Inc. — Software Security Engineer (Dec 2015 – Mar 2017)
Inherited a legacy codebase handling customer money; built static analysis tooling that traced variable flow into SQL to find injection paths — the earliest version of what became Pickle. Gate-kept every product launch; nothing shipped without passing security review.

---

### 📫 Connect
[LinkedIn](https://www.linkedin.com/in/steven-horton-66325520/)

