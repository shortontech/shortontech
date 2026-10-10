# Steven Horton

**Application security · Secure-by-design tooling · Framework-aware analysis · Developer guardrails**

I build secure-by-design developer tooling, native software, and systems that make complex behavior explicit and inspectable. My work spans framework-aware static analysis, code generation, cross-platform desktop software, and native UI architecture.

## Selected projects

| [Twinkle](https://github.com/shortontech/twinkle) | [Nickel](https://github.com/shortontech/nickel) |
| --- | --- |
| A native Rust UI engine with declarative Rust and optional JSX/TSX authoring, typed messages, responsive layout, accessible controls, controller navigation, and native presentation. Applications can use the core Rust engine without including the JavaScript executor. | [![Nickel desktop environment](assets/nickel-default-shell.png)](https://github.com/shortontech/nickel)<br><br>A Twinkle-based desktop environment for Windows and Linux with its own taskbar or dock, launcher, task switching, system controls, controller navigation, and applications. Its customizable shell is authored in TSX and rendered natively without Electron or a browser. |

### [🥒 Pickle](https://github.com/shortontech/pickle)

**Secure foundations for agentic software development**  

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

---

## Whitepapers

### [Using Agentic Tooling to Build Application-Specific AppSec Controls](https://shortontech.github.io/whitepapers/application-specific-appsec-controls/)

Application-specific security judgment can become repository-owned static checks, CI gates, analyzer plugins, review bots, and proof artifacts. AI can help build and refine those controls while security engineers retain responsibility for the underlying judgment.

### [Policy-Carrying Fields for Application-Specific Security Tooling](https://shortontech.github.io/whitepapers/policy-carrying-fields/)

Ordinary ORM fields can carry explicit expectations for visibility, mutation, logging, serialization, and auditing. Static analysis and generated metadata can then enforce that intent across an application.

### [Human Swarm Mode](https://shortontech.github.io/whitepapers/human-swarm-mode/)

Human Swarm Mode uses AI-native apprenticeship to expand technical capacity through narrow problem lanes, disciplined artifacts, and senior review. Operators learn and execute, engineers integrate, and domain experts validate assumptions and results.
