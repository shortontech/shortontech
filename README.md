# Steven Horton

**Security Engineer** · Lancaster, CA · Open to relocation  
Secure-by-design tooling · Framework-aware AppSec · Incident response · Developer guardrails

I build application security tooling for engineers who need more than scanner output. My work focuses on secure-by-design systems, framework-aware static analysis, code generation, and review artifacts that make security assumptions visible in the repository.

Recent work includes public whitepapers on application-specific AppSec controls and policy-carrying model fields, plus Pickle, an experimental Go backend generator that turns schema and access intent into code a repository can inspect, test, and keep.

---

## Whitepapers

### [Using Agentic Tooling to Build Application-Specific AppSec Controls](https://shortontech.github.io/whitepapers/application-specific-appsec-controls/)

Most AppSec tools are broad by design, but many real failures are specific to one application. This paper argues for turning repeated security judgment into repository-owned controls: static checks, CI gates, analyzer plugins, review bots, and proof artifacts that encode local invariants. The examples cover tenant boundaries, serializer exposure, webhook verification, dependency reachability, and state-transition rules.

The core idea is that AI is useful when it helps build enforcement, not when it replaces review. An agent can read a codebase, find sibling patterns, draft an invariant, generate fixtures, and iterate on false positives. The security engineer still owns judgment. The endpoint is a control the repository can run again.

### [Policy-Carrying Fields for Application-Specific Security Tooling](https://shortontech.github.io/whitepapers/policy-carrying-fields/)

This paper extends the AppSec controls argument into the model layer. Instead of leaving visibility, logging, mutation, serialization, and audit expectations scattered across code review comments or wiki pages, ordinary ORM fields can carry security intent directly. A field can say who may see it, who may mutate it, whether it may be logged, whether it can cross an API boundary, and what audit behavior it requires.

Once that intent is explicit, static analysis and generated metadata can enforce it. A diagnosis, internal risk flag, treatment plan, and audit record should not move through the application in the same way. The point is not to create a new ORM. The point is to augment the model surface developers already trust.

### [Human Swarm Mode](https://shortontech.github.io/whitepapers/human-swarm-mode/)

Human Swarm Mode is a broader workforce and technical-operations paper. It argues that AI can create more technical workers, not fewer, when used as infrastructure for AI-native apprenticeship. The model pairs senior expert review with narrow problem lanes, disciplined artifacts, and operators who learn a bounded domain deeply enough to prioritize inside it.

It separates learning, design, and validation: operators expand learning and execution capacity, engineers integrate systems, and deep domain experts validate assumptions, data, models, and interpretation. The strongest version is not “AI replaces people.” It is an accelerator for AI powered by human beings who provide priority, judgment, accountability, and escalation.

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

## 🧰 Languages and tools

**Languages:** Go, Python, TypeScript / JavaScript, PHP, SQL, C#  
**Frameworks:** Django, Laravel, Node.js, React, Next.js, Rails familiarity through security tooling  
**Security:** AppSec, threat modeling, incident response, secure SDLC, SAST/DAST, OWASP Top 10, auth/RBAC, cryptographic key management  
**Cloud / DevOps:** AWS, Docker, Kubernetes, Terraform, GitLab CI, GitHub Actions, Linux, PostgreSQL, MySQL
