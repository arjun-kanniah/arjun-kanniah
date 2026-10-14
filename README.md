# Arjun Kanniah

**Solutions architect and hands-on engineer.** I design GenAI and cloud platforms and build
them through to production: the application, the infrastructure, and the security and
release practices that keep them running.

**13+ years** across DevOps, platform engineering and software quality, from enterprise
release management for 15 product teams to architecting GenAI platforms adopted across
engineering, quality and program management.

### What I work on
- **GenAI systems:** retrieval-augmented generation, multi-agent workflows (LangChain, CrewAI,
  native function calling), document extraction pipelines, LLM evaluation, and
  provider-agnostic design across OpenAI, Gemini and Claude
- **Application architecture:** React + TypeScript, Node (Express, Fastify), Python/FastAPI,
  MongoDB, PostgreSQL, event-driven and real-time services
- **Cloud platforms:** Terraform, containers, Kubernetes/OpenShift, CI/CD and GitOps on GCP,
  Azure and AWS, with SSO, secret management and cost governance built in
- **Engineering leadership:** reference architectures and deployment blueprints adopted
  across teams, release-quality gates, and mentoring engineers

### Featured work
| Project | What it shows |
|---|---|
| [**DocPilot**](https://github.com/arjun-kanniah/docpilot)<br>[Live demo](https://docpilot.arjunkanniah.dev) | Ask questions about your documents and get streamed answers with page citations, or hand it a task in Research mode: a LangGraph researcher, analyst and writer search the library with tools, check their notes against the sources and show every step. Handles documents that disagree (newer versions win), follow-up questions, and chats limited to chosen documents. Claude, OpenAI and Gemini behind one interface. Three evaluation sets with an LLM grader measure correctness, declining when the documents don't have the answer, and evidence found; retrieval is checked in CI. FastAPI, PostgreSQL + pgvector, React + TypeScript, deployed to Cloud Run with Terraform. |
| [**FlowApprove**](https://github.com/arjun-kanniah/flowapprove)<br>[Live demo](https://flowapprove.arjunkanniah.dev) | Purchase-request approvals: requests go to the requester's manager and, above a threshold, to finance, with separation of duties enforced, live updates over WebSockets, email notifications through an outbox, and an audit log the database won't let anyone rewrite. An AI check reads the attached vendor quote and compares vendor, total and dates with the request in code. Sign-in with Microsoft accounts through Entra ID, with no client secret. Node + TypeScript (Fastify, Prisma), React, PostgreSQL, deployed to Azure Container Apps with Terraform: Key Vault, Blob Storage and managed identities, no stored keys. |
| [**cloudrun-blueprint**](https://github.com/arjun-kanniah/cloudrun-blueprint) | Terraform modules and a reusable GitHub Actions workflow for running apps on Cloud Run. Deploys use Workload Identity Federation (no key files), each app reads only its own secrets, and migrations run before every rollout. Includes a budget alert and a streaming custom domain through a Cloudflare Worker. Tested with `terraform test` against mocked providers. DocPilot is built on it. |

[LinkedIn](https://www.linkedin.com/in/arjun-kanniah/)
