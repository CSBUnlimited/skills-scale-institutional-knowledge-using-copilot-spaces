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

## Release Manager

### Role Summary
Release Managers coordinate release planning and execution so deployments are predictable, low-risk, and well-communicated across technical and business teams.

### Responsibilities
- Maintain the release calendar and release scope decisions with PM and PdM
- Confirm release readiness gates are met before production deployment
- Coordinate release sign-offs and ensure rollback plans are documented
- Lead release-day communication and post-release summaries
- Track release risks and escalate blockers quickly

### Goals
- Improve release reliability and reduce failed deployments
- Ensure every release has clear go/no-go decisions and owners
- Keep stakeholders informed before, during, and after releases

### Typical Communication
- Release readiness reviews and go/no-go meetings
- Deployment status updates in team and stakeholder channels
- Release notes and post-release summaries

### Works Closely With
- **Project Manager:** aligns timelines, dependencies, and risk escalations
- **Product Manager:** confirms release scope and customer impact priorities
- **Developers:** validates implementation status, feature flags, and technical risks
- **QA/Testing and QA Lead:** confirms quality gate outcomes and test completion
- **DevOps Engineer:** coordinates deployment sequencing, monitoring, and rollback readiness
- **Stakeholders:** communicates release windows, impact, and outcomes

---

## QA Lead

### Role Summary
QA Leads own the project test strategy and quality gates, ensuring features satisfy acceptance criteria and are fit for release.

### Responsibilities
- Define and maintain quality gates for In Review, QA, and pre-release stages
- Lead test planning, coverage strategy, and test execution priorities
- Partner with PdM and PM to clarify acceptance criteria and edge cases
- Coordinate defect triage, severity decisions, and release quality sign-off
- Report quality trends and recurring risk themes to the team

### Goals
- Prevent regressions and reduce escaped defects
- Increase confidence in release readiness decisions
- Make quality expectations explicit and repeatable

### Typical Communication
- Test strategy updates and defect triage notes
- Quality gate decisions and pass/fail rationale
- Cross-functional readouts on quality risks before release

### Works Closely With
- **Developers:** aligns on testability, bug reproduction, and fix validation
- **Project Manager:** escalates quality risks and adjusts timelines when needed
- **Product Manager:** validates acceptance criteria and customer-critical scenarios
- **Release Manager:** confirms readiness and sign-off status for releases
- **DevOps Engineer:** aligns test environments, deployment validation, and monitoring checks
- **Stakeholders:** communicates quality confidence and known risks for go/no-go decisions

---

## UX Designer

### Role Summary
UX Designers ensure solutions are usable, consistent, and aligned to customer needs from discovery through delivery.

### Responsibilities
- Lead discovery and user-flow definition with PdM and stakeholders
- Produce wireframes/prototypes and interaction specifications
- Define usability acceptance inputs and design hand-off artifacts
- Review implemented experiences with developers before release
- Capture usability feedback and recommend iterative improvements

### Goals
- Improve user satisfaction and task completion success
- Reduce rework caused by unclear or late design decisions
- Keep product and engineering aligned on user experience outcomes

### Typical Communication
- Discovery workshops, design reviews, and hand-off walkthroughs
- Annotated mockups and usability findings
- Iteration proposals based on user and stakeholder feedback

### Works Closely With
- **Product Manager:** aligns user outcomes, prioritization, and problem framing
- **Project Manager:** aligns design milestones, dependencies, and timeline trade-offs
- **Developers:** clarifies implementation details and performs implementation reviews
- **QA/Testing and QA Lead:** defines usability-focused acceptance checks and test scenarios
- **Release Manager:** highlights UX-sensitive release risks and communication needs
- **Stakeholders:** validates business and user context for major UX decisions

---

## DevOps Engineer

### Role Summary
DevOps Engineers own CI/CD, environment reliability, and operational readiness to support safe and repeatable delivery.

### Responsibilities
- Maintain and improve build, test, and deployment pipelines
- Define environment standards, observability baselines, and runbooks
- Support release execution, rollback procedures, and incident response
- Partner with teams on automation and reliability improvements
- Monitor production health and coordinate operational escalations

### Goals
- Reduce deployment friction and mean time to recovery (MTTR)
- Increase system reliability and operational visibility
- Standardize repeatable delivery practices across teams

### Typical Communication
- CI/CD health updates and deployment readiness signals
- Incident updates and post-incident action follow-ups
- Runbook changes and platform reliability recommendations

### Works Closely With
- **Developers:** improves CI reliability, infrastructure automation, and release workflows
- **Project Manager:** escalates delivery-impacting platform risks and dependencies
- **Product Manager:** explains operational constraints and release trade-offs
- **QA/Testing and QA Lead:** enables stable test environments and release verification telemetry
- **Release Manager:** executes deployment plans, rollback actions, and release monitoring
- **Stakeholders:** communicates incident impact and operational recovery status when needed

---

## Ownership & Hand-offs (lightweight RACI model)

The table below clarifies ownership for common activities. **A = Accountable**, **R = Responsible**, **C = Consulted**, **I = Informed**.

| Activity | PM | PdM | Developers | QA Lead | Release Manager | UX Designer | DevOps Engineer | Stakeholders |
|---|---|---|---|---|---|---|---|---|
| Backlog grooming | A | R | C | C | I | C | I | I |
| Acceptance criteria definition | C | A | C | R | I | R | I | C |
| Risk register updates | A | C | C | C | C | I | C | I |
| Release readiness review | C | C | R | R | A | I | R | I |
| Incident communications | A | C | C | C | R | I | R | I |
| Retrospective action tracking | A | C | R | R | C | C | C | I |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
