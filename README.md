# Arjun Kanniah

**Solutions architect and hands-on engineer.** I build GenAI systems that hold up in
production: retrieval and agents with evaluations that show they work, on cloud
infrastructure that's secure, automated and cheap to run.

**13+ years** across DevOps, platform engineering and software quality, from enterprise
release management for 15 product teams to architecting GenAI platforms adopted across
engineering, quality and program management. That work lives in private company
repositories; the projects below are built from scratch in public to show how I work.

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
| [**DocPilot**](https://github.com/arjun-kanniah/docpilot)<br>[Live demo](https://docpilot.arjunkanniah.dev) | Ask questions about your documents and get streamed answers with page citations, or hand it a task in Research mode: a LangGraph researcher, analyst and writer search the library with tools, check their notes against the sources and show every step. Handles documents that disagree (newer versions win), follow-up questions, and chats limited to chosen documents. Claude, OpenAI and Gemini behind one interface. Three evaluation sets with an LLM grader measure correctness, declining when the documents don't have the answer, and evidence found; retrieval is checked in CI and [benchmarked on public datasets of up to 57K documents](https://github.com/arjun-kanniah/docpilot#retrieval-at-scale) (hybrid search, rerankers, embedders, filtered search), with significance tests. FastAPI, PostgreSQL + pgvector, React + TypeScript, deployed to Cloud Run with Terraform. |
| [**FlowApprove**](https://github.com/arjun-kanniah/flowapprove)<br>[Live demo](https://flowapprove.arjunkanniah.dev) | Purchase-request approvals: requests go to the requester's manager and, above a threshold, to finance, with separation of duties enforced, live updates over WebSockets, email notifications through an outbox, and an audit log the database won't let anyone rewrite. An AI check reads the attached vendor quote and compares vendor, total and dates with the request in code. Sign-in with Microsoft accounts through Entra ID, with no client secret. Node + TypeScript (Fastify, Prisma), React, PostgreSQL, deployed to Azure Container Apps with Terraform: Key Vault, Blob Storage and managed identities, no stored keys. |
| [**cloudrun-blueprint**](https://github.com/arjun-kanniah/cloudrun-blueprint) | Terraform modules and a reusable GitHub Actions workflow for running apps on Cloud Run. Deploys use Workload Identity Federation (no key files), each app reads only its own secrets, and migrations run before every rollout. Includes a budget alert and a streaming custom domain through a Cloudflare Worker. Tested with `terraform test` against mocked providers. DocPilot is built on it. |

[LinkedIn](https://www.linkedin.com/in/arjun-kanniah/)
