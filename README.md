# Steven Horton

**Security Engineer** · Lancaster, CA · Open to relocation  
Secure-by-design tooling · Framework-aware AppSec · Incident response · Developer guardrails

I’m a security engineer with 16 years across fintech, e-commerce, and AI-adjacent systems. I like security work that makes the vulnerable path hard to take by accident: generated constraints, explicit authorization posture, framework-aware analysis, and tools developers can run before bad patterns reach production.

My strongest work is at the boundary between application security and developer tooling: routes, middleware, authorization, ORM usage, serializers, request validation, data flow, and the places where real vulnerabilities hide between those layers.

---

## 🥒 Pickle

**Secure foundations for agentic software development**  
[github.com/shortontech/pickle](https://github.com/shortontech/pickle)

Pickle is a secure-by-design Go code generation framework and research project for apps that need to be understandable, auditable, and safe for humans and AI agents to modify.

It turns a declared application model into plain, idiomatic Go with explicit security posture and no runtime dependency on Pickle. The goal is not to invent a clever framework for its own sake; the goal is to make common AppSec failure modes structurally difficult to express and easy to verify.

Pickle generates and verifies:

- typed request binding and validation
- parameterized query builders
- explicit route and middleware wiring
- ownership-scoped data access
- RBAC and gated actions
- GraphQL exposure rules
- sealed/encrypted field handling
- immutable audit-table integrity checks
- framework-level static analysis through `pickle squeeze`
- conventional Go export through `pickle export`

`pickle export` packages the same generated Go used by normal Pickle builds into a conventional application layout, so teams can keep the security guarantees without betting their application’s future on a custom framework runtime.

---

## 🦅 TelHawk

**Security telemetry and event tooling for high-context review**  
[github.com/telhawk-systems/telhawk-stack](https://github.com/telhawk-systems/telhawk-stack)

TelHawk is an event management and security telemetry project built around one principle: alerts and events are only useful when they carry the right context for a human or AI reviewer to act on them.

The project includes SIEM-oriented components, structured event ingestion, and supporting infrastructure for review workflows that prioritize clarity over dashboards full of noise.

Related work includes TelHawk Proxy: a first-party telemetry reverse proxy with HMAC-authenticated routing and pluggable sinks for Kafka, PostgreSQL, and NDJSON.

---

## 🔍 Security tooling focus

I build tools that reason across framework boundaries instead of scanning files in isolation.

The vulnerability classes I care most about usually live in the seams:

- an authenticated route with an unscoped ORM query
- a serializer or resource exposing fields it should not
- a middleware chain that looks protected but no longer enforces the intended guard
- a write path with strong authorization paired with a read path that is weaker
- a generated or framework convention that quietly became the security contract

My recent work focuses on framework-aware analysis that connects routes, auth posture, ORM behavior, serializers, schema, and data flow into one reviewable picture.

---

## 🛠️ What I like building

- secure-by-design frameworks and code generators
- static analysis over real application semantics
- AppSec tools that produce proof, not just alerts
- CI guardrails developers can trust
- systems that make secure implementation the default path
- incident visibility that turns “we think something happened” into “here is the path”

---

## ⚡ Selected background

- Built observability and real-time analytics that made a crypto exchange breach immediately visible; helped identify the attack vector, contain the incident, and restore operations with zero customer impact.
- Built framework-aware static analysis tooling using tree-sitter to reason across routes, authentication, ORM queries, serializers, and data flow in Django, Laravel, and Rails applications.
- Built fraud-detection and attribution tooling that blocked 52%+ of incoming bot traffic and protected millions in annual marketing spend.
- Enforced automated SAST, DAST, and dependency scanning in GitLab pipelines without manual review workarounds.
- Built and secured fintech, marketplace, payments, telemetry, and analytics systems across Go, Python, TypeScript, PHP, SQL, AWS, Docker, and Kubernetes.

---

## 🧰 Languages and tools

**Languages:** Go, Python, TypeScript / JavaScript, PHP, SQL, C#  
**Frameworks:** Django, Laravel, Node.js, React, Next.js, Rails familiarity through security tooling  
**Security:** AppSec, threat modeling, incident response, secure SDLC, SAST/DAST, OWASP Top 10, auth/RBAC, cryptographic key management  
**Cloud / DevOps:** AWS, Docker, Kubernetes, Terraform, GitLab CI, GitHub Actions, Linux, PostgreSQL, MySQL

---

## 🧭 How I think about security

Security should not depend on every developer remembering every rule every time.

The best security work changes the shape of the system: safer defaults, explicit contracts, generated constraints, fast feedback, and artifacts that explain why a finding is real. Review still matters, but review gets a lot better when the codebase is built to make the important paths visible.
