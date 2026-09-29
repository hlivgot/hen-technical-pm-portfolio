# Technical Program Operating Model

This document describes how I manage technical programs across product, engineering, QA, data, AI, and operations.

## Operating Principle

A technical program is healthy when every important piece of work has:

- A clear owner.
- A clear decision path.
- A visible dependency map.
- A measurable success metric.
- A release or delivery checkpoint.
- A known risk and recovery path.

## End-to-End Flow

| Stage | Main Question | TPM / Product Ops Responsibility | Evidence |
|---|---|---|---|
| Problem framing | What problem are we solving? | Align product need, user pain, scope, and success criteria | Problem statement, success metrics |
| Discovery | What do we need to learn before building? | Identify assumptions, unknowns, data needs, and risks | Assumption log, discovery plan |
| Planning | What will be built, by whom, and when? | Build roadmap, milestones, dependencies, and RAID log | Roadmap, dependency map, RAID log |
| Execution | Is work moving according to plan? | Run cadence, unblock teams, track plan vs actual | Sprint readiness, status reports |
| Release | Are we ready to ship safely? | Coordinate QA, go/no-go, rollback, comms, support readiness | Release checklist, go/no-go log |
| Operation | Is the product working in production? | Monitor incidents, KPIs, adoption, cost, and quality | Dashboard, incident log |
| Learning | What should change next cycle? | Run post-launch review and update operating model | Postmortem, action tracker |

## Key Interfaces

| Function | What They Own | What I Need To Clarify |
|---|---|---|
| Product | Problem, user value, priority | Scope, tradeoffs, success metrics |
| Engineering | Technical design, implementation | Dependencies, estimates, technical risk |
| QA | Test strategy and quality gates | Acceptance criteria, regression risk |
| Data | Data model, pipelines, quality | Source reliability, freshness, ownership |
| DevOps / Platform | Environments, deployment, monitoring | CI/CD, rollback, observability, cost |
| Security / Legal | Risk and compliance | Review requirements and approval gates |
| Support / Operations | User impact and incident handling | Launch comms, escalation path, known issues |

## What I Monitor

- Scope changes and decision latency.
- Cross-team dependencies.
- Critical path and blocked work.
- QA readiness and defect trends.
- Release risk and rollback readiness.
- Production health, adoption, and user feedback.
- AI-specific quality: eval results, hallucination risk, latency, cost, and drift.

## Executive Reporting Format

Every executive update should answer:

1. Where are we versus plan?
2. What changed since the last update?
3. What is at risk?
4. What decision is needed, by whom, and by when?
5. What happens if no decision is made?

