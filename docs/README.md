# OctoAcme Project Management Docs

Welcome! This repository centralizes the project management processes and templates used by OctoAcme teams to plan, execute, and improve projects. These docs support consistent, repeatable delivery and effective knowledge sharing across teams.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Project Lifecycle Overview](#project-lifecycle-overview)
   - [Phase 1: Initiation](#phase-1-initiation)
   - [Phase 2: Planning](#phase-2-planning)
   - [Phase 3: Execution & Tracking](#phase-3-execution--tracking)
   - [Phase 4: Release & Deployment](#phase-4-release--deployment)
   - [Phase 5: Close & Retrospective](#phase-5-close--retrospective)
3. [Core Roles & Responsibilities](#core-roles--responsibilities)
4. [Key Workflows & Communication](#key-workflows--communication)
5. [Quality Assurance Practices](#quality-assurance-practices)
6. [Continuous Improvement](#continuous-improvement)
7. [Quick Reference Checklists](#quick-reference-checklists)
8. [Documentation Index](#documentation-index)

---

## Introduction

OctoAcme follows an iterative, evidence-driven project management approach built on five core principles:

- **Customer-first** — prioritize customer value and usability.
- **Iterative delivery** — deliver small, testable increments.
- **Clear ownership** — each project has a named Project Manager (PM) and Product Lead.
- **Data-informed decisions** — measure impact and iterate based on evidence.
- **Psychological safety** — encourage feedback and learning at every stage.

This documentation set is the single source of truth for how OctoAcme plans, executes, and ships projects. It is intended as an onboarding resource for new team members and a reference guide for experienced practitioners.

---

## Project Lifecycle Overview

OctoAcme projects follow a five-phase lifecycle. Each phase has defined goals, deliverables, and decision gates to keep teams aligned and work moving forward.

### Phase 1: Initiation

**Goal:** Validate the business need and align stakeholders before committing resources.

Key activities:
- Complete a **Project One-pager** with a problem statement, goal, success metrics, stakeholder list, and initial timeline.
- Confirm team availability and resource needs.
- Hold a sponsor / stakeholder alignment meeting.
- Decide go/no-go for planning.

**Decision gate:** Move to Planning when success metrics are clear, stakeholders agree on priority, and team availability is confirmed.

📄 [Project Initiation Guide](octoacme-project-initiation.md)

---

### Phase 2: Planning

**Goal:** Turn an approved initiative into an actionable backlog and release plan.

Key activities:
- Run a kickoff meeting with stakeholders and the delivery team.
- Build a prioritized backlog with acceptance criteria and estimates.
- Define the **Definition of Done (DoD)**.
- Identify dependencies, integration points, and initial risks.
- Create a release plan and milestone map.

**Decision gate:** Planning is complete when the backlog is prioritized, the release timeline is agreed, and the initial test plan is drafted.

📄 [Project Planning Guide](octoacme-project-planning.md)

---

### Phase 3: Execution & Tracking

**Goal:** Deliver working increments while maintaining quality and transparency.

Key activities:
- Hold daily standups (15 min) and weekly delivery syncs.
- Manage work on the project board (Backlog → Ready → In Progress → In Review → QA → Done).
- Follow the pull request workflow: small PRs (≤ 400 lines), CI checks, at least one approval before merge.
- Update the Risk Register weekly.
- Escalate blockers through the defined path: Team → PM → Product Lead → Sponsor.

📄 [Execution & Tracking Guide](octoacme-execution-and-tracking.md)
📄 [Risk Management & Communication Guide](octoacme-risks-and-communication.md)

---

### Phase 4: Release & Deployment

**Goal:** Deploy features to production safely and with full stakeholder awareness.

Key activities:
- Confirm all acceptance criteria are met and PRs are merged.
- Verify passing CI, security scans, and smoke tests on staging.
- Draft release notes and document a rollback plan.
- Deploy via automated pipeline (preferred), run post-deploy verifications.
- Announce the release to stakeholders and support teams.

Release types: **Patch** (hotfixes), **Minor** (incremental features), **Major** (significant or breaking changes).

📄 [Release & Deployment Guide](octoacme-release-and-deployment.md)

---

### Phase 5: Close & Retrospective

**Goal:** Capture learnings and convert them into actionable improvements.

Key activities:
- Run a retrospective (45–75 min) after each sprint, release, or milestone.
- Structure: What went well · What could be improved · Action items (owner + due date) · Follow-up on previous actions.
- Add 2–3 prioritized action items to the backlog with clear owners.
- Review outstanding actions in the weekly PM sync.

📄 [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md)

---

## Core Roles & Responsibilities

OctoAcme projects rely on three primary roles working in close collaboration.

### Project Manager (PM)
Coordinates delivery activities, manages schedules, risks, and cross-team communication.

| Responsibility | Details |
|---|---|
| Project plans & timelines | Create and maintain plans with clear milestones |
| Risk & dependency management | Own the Risk Register and escalate blockers |
| Meeting facilitation | Kickoffs, planning sessions, retrospectives |
| Status reporting | Weekly updates using the standard status template |
| Stakeholder alignment | Ensure consistent communication across all groups |

### Product Manager (PdM)
Defines what should be built to deliver customer and business value.

| Responsibility | Details |
|---|---|
| Problem statements & metrics | Define success criteria and measure outcomes |
| Backlog prioritization | Own the roadmap and prioritize features |
| Trade-off decisions | Collaborate with engineering on scope and constraints |
| Solution validation | Use data and user research to confirm impact |

### Developer
Implements and delivers reliable, tested software components.

| Responsibility | Details |
|---|---|
| Feature implementation | Build to acceptance criteria and quality standards |
| Testing & documentation | Write unit/integration tests, maintain docs |
| Code & design reviews | Participate in PRs and technical design discussions |
| Risk identification | Flag technical risks early in planning and execution |

📄 [Roles & Personas Reference](octoacme-roles-and-personas.md)

---

## Key Workflows & Communication

### Communication Cadence

| Cadence | Who | Purpose |
|---|---|---|
| Daily standup (15 min) | Delivery team | Progress, blockers, dependencies |
| Weekly PM ↔ PdM sync | PM + Product Lead | Alignment, risk review, decisions |
| Weekly delivery sync | All team + stakeholders | Show progress, flag risks |
| Monthly stakeholder update | PM + broader stakeholders | High-level status and roadmap |
| Ad-hoc escalations | As needed | Business-impacting issues |

### Weekly Status Template

```
Progress this week:
Next steps:
Risks & blockers:
Ask / decisions needed:
```

### Risk Register Fields

| Field | Description |
|---|---|
| ID | Unique identifier |
| Description | What is the risk? |
| Impact | High / Med / Low |
| Likelihood | High / Med / Low |
| Owner | Who is responsible? |
| Mitigation plan | How will it be addressed? |
| Status | Open / In Progress / Resolved |

### Escalation Path

```
Team-level triage (daily standup)
  ↓ (unresolved)
PM escalates to Product Lead + dependent teams
  ↓ (business-impacting)
Sponsor-level escalation
```

📄 [Risk Management & Communication Guide](octoacme-risks-and-communication.md)

---

## Quality Assurance Practices

Quality is embedded throughout execution — not treated as a gate at the end.

- **Unit tests** required for all new logic.
- **Integration tests** for component interactions where applicable.
- **End-to-end smoke tests** for critical flows before every release.
- **Security scanning** runs automatically in CI.
- **Manual QA** for feature acceptance when automated coverage is insufficient.
- **Code review**: all PRs require at least one approval; CI must pass before merge.
- **Metrics & dashboards**: track velocity, burndown, error rates, and latency against success metrics defined in the Project One-pager.

📄 [Execution & Tracking Guide](octoacme-execution-and-tracking.md)

---

## Continuous Improvement

OctoAcme teams use structured retrospectives after every sprint, release, or milestone to drive measurable improvement.

- Follow the **What went well / What could be improved / Action items** format.
- Timebox retrospectives to 45–75 minutes; use anonymous idea boards when helpful.
- Commit to **2–3 prioritized action items** per retrospective with owners and due dates.
- Track actions in the project backlog; review progress in weekly PM syncs.
- Measure the impact of improvements and celebrate incremental wins.

📄 [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md)

---

## Quick Reference Checklists

### ✅ Initiation Checklist
- [ ] One-pager completed and reviewed by Product Lead
- [ ] Stakeholder alignment confirmed
- [ ] Go/no-go decision made
- [ ] Repo / project board skeleton created

### ✅ Planning Checklist
- [ ] Kickoff meeting held
- [ ] Backlog prioritized and estimated
- [ ] Release timeline and milestones agreed
- [ ] Definition of Done documented
- [ ] Initial test / QA plan drafted

### ✅ Execution Checklist
- [ ] Branching and PR conventions documented
- [ ] CI configured for tests and linting
- [ ] Regular demos scheduled
- [ ] Risk Register updated weekly

### ✅ Release Checklist
- [ ] All acceptance criteria met, PRs merged
- [ ] CI and security scans passing
- [ ] Smoke tests passed on staging
- [ ] Release notes drafted
- [ ] Rollback plan documented
- [ ] Stakeholders notified

### ✅ Retrospective Checklist
- [ ] Retrospective scheduled within one week of milestone
- [ ] All team members invited
- [ ] 2–3 action items captured with owners and due dates
- [ ] Actions added to project backlog

---

## Documentation Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level intro to OctoAcme's PM approach, principles, and key artifacts |
| [Roles & Personas](octoacme-roles-and-personas.md) | Definitions and responsibilities for PM, PdM, and Developer roles |
| [Project Initiation Guide](octoacme-project-initiation.md) | Steps to validate and authorize new projects |
| [Project Planning Guide](octoacme-project-planning.md) | Turning an approved initiative into an actionable plan |
| [Execution & Tracking Guide](octoacme-execution-and-tracking.md) | Day-to-day workflow, board management, PR practices, and metrics |
| [Risk Management & Communication Guide](octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication templates |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release types, deployment checklist, rollback, and release notes |
| [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md) | Running retrospectives and tracking improvement actions |

---

*This README is maintained by the OctoAcme project management team. To suggest changes, open an issue or pull request in this repository.*
