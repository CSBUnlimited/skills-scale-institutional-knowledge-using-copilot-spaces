# OctoAcme Project Management Docs

Welcome! This README is the central entry point for OctoAcme's project management documentation. It summarizes our approach and provides direct links to all key process guides.

## Overview

OctoAcme's project management approach follows a lightweight, end-to-end lifecycle designed for consistent delivery across cross-functional teams. Work progresses through five phases: **initiation** (confirm the problem, stakeholders, success metrics, and a go/no-go decision), **planning** (turn an approved initiative into milestones, a prioritized backlog, estimates, dependencies, and a clear Definition of Done), **execution** (build and track work through a shared board and PR workflow), **release** (deploy with checklists, verification, and communications), and **close/retrospective** (capture learnings and feed improvements back into the backlog and process docs).

Clear ownership and well-defined personas are central to the process. A named **Project Manager (PM)** coordinates delivery mechanics—timeline, risks, dependencies, and stakeholder communications—while a **Product Manager (PdM)** defines outcomes, prioritizes work, and measures success. **Developers** implement shippable increments with a focus on testability and maintainability, and **QA/Testing** validates acceptance criteria and quality for releases. Stakeholders contribute inputs and approvals, with alignment reinforced through documented artifacts like the project one-pager/charter, backlog items with acceptance criteria, a risk register, and retrospective action items.

Communication is handled through a predictable team rhythm and explicit escalation paths. Teams use short **daily standups** to surface blockers, a **weekly delivery sync** to demonstrate progress and flag risks, and demos at sprint or milestone boundaries. Stakeholder communication emphasizes a "single source of truth" (such as a project README or release doc) plus regular status updates using a standard weekly template (progress, next steps, risks/blockers, and asks/decisions). Risks and cross-team dependencies are tracked in a risk register and escalated progressively from team triage to PM/Product Lead and, if needed, sponsor-level escalation.

Quality assurance is built into both execution and release practices. During delivery, teams favor **small pull requests**, include issue links and acceptance criteria in PR descriptions, run automated tests and linting in CI, and require at least one approval before merging. Testing expectations include unit tests for new logic, integration tests where applicable, and end-to-end smoke tests for critical flows, supplemented by security scanning in CI and manual QA for feature acceptance when needed. Releases follow a standardized checklist (acceptance criteria met, CI/security checks passing, release notes and rollback plan prepared, staged deployment and post-deploy verification), with an incident/rollback playbook and a blameless retrospective loop to drive continuous improvement.

---

## Key Workflows

| Phase | Description |
|---|---|
| **Initiation** | Define the problem, identify stakeholders, set success metrics, and pass a go/no-go decision gate. |
| **Planning** | Refine scope, build a prioritized backlog with acceptance criteria, estimate work, map dependencies, and establish a release plan and risk register. |
| **Execution & Tracking** | Build and iterate through daily standups, a shared project board, and a structured PR workflow with CI checks and peer review. |
| **Release** | Deploy using a pre-release checklist, staged rollout, post-deploy verification, and a documented rollback/incident playbook. |
| **Retrospective & Continuous Improvement** | Run blameless retrospectives, capture action items with owners and due dates, and feed learnings back into the backlog and process docs. |

---

## Personas / Roles

| Role | Summary |
|---|---|
| **Project Manager (PM)** | Coordinates delivery, manages timeline, risks, dependencies, and cross-team communication. |
| **Product Manager (PdM)** | Defines the product vision, prioritizes the backlog, and measures customer outcomes. |
| **Developers** | Implement features, write tests and docs, participate in design and code review. |
| **QA / Testing** | Validate acceptance criteria, run test suites, and sign off on release quality. |
| **Stakeholders** | Provide requirements, approvals, and strategic direction; receive regular status updates. |

---

## Communication Strategies

- **Cadences:** Daily standups to surface blockers; weekly delivery sync to review progress and risks; sprint/milestone demos for stakeholder alignment; monthly stakeholder updates.
- **Single Source of Truth:** All project status, decisions, and artifacts are maintained in the project repo (README, risk register, board). Duplicated or stale information is avoided.
- **Weekly Status Template:** Progress this week → Next steps → Risks/blockers → Asks/decisions needed.
- **Escalation Path:** Team self-triage → PM/Product Lead → Sponsor/executive escalation for unresolved blockers; security incidents have a separate, immediate escalation track.

---

## Quality Assurance Practices

- **PR Workflow:** Small, focused pull requests linked to issues; PR descriptions include acceptance criteria; CI must pass (tests, lint, security scans) before merge; at least one peer approval required.
- **Testing Types:** Unit tests for all new logic; integration tests where applicable; end-to-end smoke tests for critical user flows.
- **CI / Security:** Automated pipelines run on every PR; security scanning is included in CI; failures block merge.
- **Release Checklists:** Acceptance criteria verified; CI and security checks green; release notes drafted; rollback plan documented; staged deployment followed by post-deploy verification.

---

## Documentation Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, roles, key artifacts, lifecycle, and communication cadence. |
| [Project Initiation](octoacme-project-initiation.md) | One-pager template, stakeholder and communication plan, initial risks, and decision gate. |
| [Project Planning](octoacme-project-planning.md) | Kickoff, backlog with acceptance criteria, estimation, Definition of Done, dependencies, release plan, and risk register. |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Team rhythm (standups, delivery sync, demos), project board workflow, PR workflow, QA expectations, and escalation levels. |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register structure and lifecycle, stakeholder communications, weekly status template, escalation path, and security incident note. |
| [Release & Deployment](octoacme-release-and-deployment.md) | Release types, pre-release requirements, deployment checklist, rollback/incident playbook, and release notes template. |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective structure, action items with owners and dates, backlog integration, and team culture. |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed role summaries, responsibilities, goals, and typical communication patterns for each persona. |

---

> For questions or suggestions, open an issue in this repository or propose a change via pull request.
