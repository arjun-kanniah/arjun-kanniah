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
- **Application architecture:** React + TypeScript, Node/Express, Python/FastAPI,
  MongoDB, PostgreSQL, event-driven and real-time services
- **Cloud platforms:** Terraform, containers, Kubernetes/OpenShift, CI/CD and GitOps on GCP,
  Azure and AWS, with SSO, secret management and cost governance built in
- **Engineering leadership:** reference architectures and deployment blueprints adopted
  across teams, release-quality gates, and mentoring engineers

### Featured work
| Project | What it shows |
|---|---|
| [**DocPilot**](https://github.com/arjun-kanniah/docpilot)<br>[Live demo](https://docpilot.arjunkanniah.dev) | Ask questions about your documents and get streamed answers with page citations. FastAPI, PostgreSQL + pgvector, React + TypeScript. Claude, OpenAI and Gemini behind one provider interface, chosen per request. An evaluation set with an LLM grader measures correctness and whether it declines when the documents don't have the answer; retrieval quality is checked in CI. Deployed to Cloud Run with Terraform and GitHub Actions. |
| [**cloudrun-blueprint**](https://github.com/arjun-kanniah/cloudrun-blueprint) | Terraform modules and a reusable GitHub Actions workflow for running apps on Cloud Run. Deploys use Workload Identity Federation (no key files), each app reads only its own secrets, and migrations run before every rollout. Includes a budget alert and a streaming custom domain through a Cloudflare Worker. Tested with `terraform test` against mocked providers. DocPilot is built on it. |

[LinkedIn](https://www.linkedin.com/in/arjun-kanniah/)
