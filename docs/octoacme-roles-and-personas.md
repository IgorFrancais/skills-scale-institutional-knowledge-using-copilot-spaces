# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers empathize with users and translate product requirements into intuitive, accessible experiences. They advocate for usability throughout the project lifecycle.

### Responsibilities
- Translate requirements into wireframes, prototypes, and design specifications
- Conduct usability testing and synthesize findings into actionable recommendations
- Advocate for accessibility and inclusive design standards
- Maintain a shared design system and pattern library
- Participate in sprint planning to surface design constraints early

### Goals
- Deliver experiences that are intuitive, accessible, and delightful
- Reduce rework by aligning design and engineering intent early
- Continuously improve UX quality based on real user feedback

### Typical Communication
- Design reviews and prototype walkthroughs with Product Managers and Developers
- Usability test reports shared with the broader team
- Async design feedback via PR comments or design tool annotations

### Interactions with Existing Roles
| Role | Nature of Interaction |
|---|---|
| Product Manager (PdM) | Receives requirements and success criteria; provides design concepts for validation |
| Project Manager (PM) | Flags design-related risks or timeline impacts; participates in planning ceremonies |
| Developers | Hands off design specs and answers implementation questions during build |

---

## Data Analyst

### Role Summary
Data Analysts turn raw data into actionable insights that inform product priorities and measure project outcomes. They support both strategic decisions and day-to-day execution.

### Responsibilities
- Define, instrument, and track key product and delivery metrics
- Support experiment design (A/B tests, feature flags) and analyze results
- Visualize and communicate findings to technical and non-technical stakeholders
- Build and maintain dashboards and reporting pipelines
- Identify data quality issues and work with engineers to resolve them

### Goals
- Ensure decisions are grounded in evidence rather than assumptions
- Provide timely, trustworthy data to support roadmap and delivery choices
- Reduce time-to-insight through scalable reporting infrastructure

### Typical Communication
- Regular metrics reviews with Product Managers and Project Managers
- Ad-hoc analysis requests from any team member
- Written summaries and dashboards shared in team channels

### Interactions with Existing Roles
| Role | Nature of Interaction |
|---|---|
| Product Manager (PdM) | Delivers insights to inform prioritization and outcome measurement |
| Project Manager (PM) | Provides progress signals, risk indicators, and delivery metrics |
| Developers | Collaborates on instrumentation, logging, and data pipeline work |

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the CI/CD, infrastructure, and observability systems that enable reliable, frequent delivery. They act as the bridge between development and production operations.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines and deployment automation
- Provision and manage infrastructure using infrastructure-as-code practices
- Ensure monitoring, alerting, and on-call runbooks are in place
- Support performance optimization, capacity planning, and incident response
- Champion security and compliance requirements in the delivery pipeline

### Goals
- Minimize deployment risk and mean-time-to-recovery (MTTR)
- Enable fast, repeatable, and auditable releases
- Keep environments stable and developer productivity high

### Typical Communication
- Release coordination meetings with Project Managers and Developers
- Incident post-mortems and runbook updates shared with the full team
- Pipeline and infrastructure change notifications via automated tooling

### Interactions with Existing Roles
| Role | Nature of Interaction |
|---|---|
| Project Manager (PM) | Coordinates release windows and communicates deployment readiness |
| Developers | Partners on build tooling, environment parity, and deployment workflows |
| Product Manager (PdM) | Surfaces infrastructure constraints that may affect roadmap timing |

---

## Customer Success Manager

### Role Summary
Customer Success Managers (CSMs) bring the voice of the customer into every project phase, ensuring delivered features genuinely solve customer problems and that customers are set up for long-term success.

### Responsibilities
- Gather, synthesize, and relay qualitative customer feedback to the product and engineering team
- Support post-launch customer onboarding and adoption activities
- Track customer satisfaction metrics (NPS, CSAT, churn signals)
- Identify expansion opportunities and surface them to the Product Manager
- Act as an escalation point for urgent customer issues that require product attention

### Goals
- Maximize customer adoption and retention
- Close the loop between customer feedback and product improvements
- Ensure customers realize the full value of delivered features

### Typical Communication
- Regular syncs with Product Managers to share feedback trends
- Post-launch check-ins with Developers on customer-reported issues
- Customer health reports distributed to Project Managers and leadership

### Interactions with Existing Roles
| Role | Nature of Interaction |
|---|---|
| Product Manager (PdM) | Shares customer feedback and adoption data to drive prioritization |
| Project Manager (PM) | Communicates post-launch status and flags any delivery gaps affecting customers |
| Developers | Escalates high-priority customer-reported bugs and validates fixes |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [RACI: Roles & Responsibilities](octoacme-roles-and-responsibilities-raci.md) for a summary of who is Responsible, Accountable, Consulted, and Informed across key ceremonies and artifacts.

