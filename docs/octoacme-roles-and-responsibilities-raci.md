# OctoAcme RACI: Roles & Responsibilities

This document summarizes who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for the key ceremonies and artifacts in OctoAcme projects.

> For full role descriptions, see [OctoAcme Personas](octoacme-roles-and-personas.md).

---

## RACI Key

| Letter | Meaning |
|--------|---------|
| **R** | **Responsible** – does the work |
| **A** | **Accountable** – owns the outcome (one per row) |
| **C** | **Consulted** – provides input before/during |
| **I** | **Informed** – notified of decisions/outcomes |

---

## RACI Matrix

| Ceremony / Artifact | Project Manager | Product Manager | Developers | UX Designer | Data Analyst | DevOps Engineer | Customer Success Manager |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **Project Charter / One-pager** | A/R | C | C | C | C | C | I |
| **Backlog Refinement** | C | A/R | R | C | C | I | C |
| **Sprint / Iteration Planning** | A/R | C | R | R | I | I | I |
| **UX Design Review** | I | C | C | A/R | I | I | I |
| **Definition of Done (DoD)** | A/R | C | R | C | I | R | I |
| **Risk Register** | A/R | C | C | I | C | C | I |
| **Release Plan** | A/R | C | R | I | I | R | C |
| **Deployment / Release** | C | I | R | I | I | A/R | I |
| **Metrics & KPI Dashboard** | I | C | C | I | A/R | I | C |
| **Post-launch Customer Review** | I | C | C | I | C | I | A/R |
| **Retrospective** | A/R | C | R | R | C | R | I |
| **Status Report / Stakeholder Update** | A/R | C | I | I | I | I | I |

---

## Cross-functional Handoff Checkpoints

Use these checkpoints to confirm key handoffs between roles are completed before moving to the next project phase.

### Initiation → Planning
- [ ] Project Manager has shared the draft Charter with Product Manager and all relevant roles for input
- [ ] UX Designer has been briefed on the problem statement and user goals
- [ ] Data Analyst has been looped in on success metrics and measurement approach

### Planning → Execution
- [ ] UX Designer has completed and shared wireframes/prototypes with Developers
- [ ] DevOps Engineer has confirmed environment and pipeline readiness
- [ ] Data Analyst has instrumentation requirements documented and assigned
- [ ] Risk Register has been reviewed and mitigations assigned

### Execution → Release
- [ ] DevOps Engineer confirms deployment runbook is ready and reviewed
- [ ] Customer Success Manager has been briefed on the upcoming release and customer communication plan
- [ ] Data Analyst has confirmed dashboards/alerts are in place for post-launch monitoring
- [ ] Product Manager has signed off on acceptance criteria

### Release → Close
- [ ] Customer Success Manager has confirmed customer onboarding/comms have been sent
- [ ] Data Analyst has validated post-launch metrics against targets
- [ ] Retrospective has been facilitated by Project Manager with all roles represented
- [ ] Action items from retrospective are assigned and tracked in the backlog
