# Infra Agents: Simulated DevOps Pipelines via AI Agent Autonomy

This project explores the feasibility of autonomous DevOps agents generating infrastructure systems, commit activity, CI/CD workflows, and observability scaffolds — as if a real human Principal Engineer were operating over a multi-month window.

> 🧠 Core concept: simulate *what a DevOps AI would do* if instructed to build, track, and maintain infrastructure over a 6-month production arc.

---

## 🧠 Goal

To test the boundaries of AI-generated DevOps outputs across:

- IaC (Terraform, Pulumi, CDKTF)
- CI/CD pipelines (GitHub Actions, CircleCI, Drone)
- Secrets management (Vault, SOPS, KMS)
- K8s orchestration (Helm, ArgoCD, GitOps)
- Observability tooling (Prometheus, Grafana, OpenTelemetry)
- ML pipeline scaffolding (MLFlow, BentoML, DVC, Ray Serve)
- GitHub signal: commits, pull requests, issues, timelines

---

## 🔁 Method

1. Designed 20 simulated repositories covering core DevOps and MLOps domains
2. Injected realistic commit histories with backdated timestamps (Feb–July 2025)
3. Auto-generated `.github/workflows` pipelines per repo
4. Created Markdown documentation, CI setups, and fake PRs/issues
5. Tracked behavior of contribution graph and commit visibility
6. Evaluated believability of agent-generated timelines

---

## 🤖 Agent Design

```bash
agents/
├── commit_agent.py         # generates commit messages and backdated activity
├── terraform_writer.py     # outputs Terraform boilerplate per stack
├── workflow_generator.py   # builds CI/CD pipeline templates
├── observability_agent.py  # sets up otel collectors, alerts, dashboards
├── mlops_synth.py          # builds DVC/MLFlow scaffolds
