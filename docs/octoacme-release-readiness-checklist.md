# OctoAcme — Release Readiness Checklist

## Purpose
Provide a reusable, role-based checklist to confirm release readiness before deployment.

## Release Types
- **Patch:** urgent fixes for production issues, narrow scope
- **Minor:** incremental features and improvements
- **Major:** broad changes with elevated coordination and communication needs

## Readiness Gates

### Gate 1: Scope and Planning
- [ ] Release type is identified (Patch / Minor / Major)
- [ ] Included work items are linked and accepted by PdM
- [ ] Dependencies and risks are reviewed by PM and Release Manager

### Gate 2: Quality and Security
- [ ] Acceptance criteria met for included items
- [ ] CI checks pass (tests, linting, security scans)
- [ ] QA Lead confirms quality gate outcomes and unresolved defects are dispositioned

### Gate 3: Operational Readiness
- [ ] Rollback plan is documented and validated
- [ ] Monitoring, alerts, and dashboards are confirmed by DevOps
- [ ] Release notes and stakeholder communication draft are ready

### Gate 4: Go / No-Go
- [ ] Final readiness review completed
- [ ] Required sign-offs are recorded
- [ ] Deployment window is confirmed (if required)

## Required Sign-offs

| Role | Sign-off Required | Notes |
|---|---|---|
| Project Manager | Yes | Timeline/dependency and risk alignment |
| Product Manager | Yes | Scope and customer-impact validation |
| QA Lead | Yes | Quality gate and defect-risk confidence |
| Release Manager | Yes | Final release readiness owner |
| DevOps Engineer | Yes | Deployment and rollback operational readiness |
| Developers | As needed | Technical readiness for owned changes |
| Stakeholders | Major only | Business readiness and communication alignment |

## Rollback Plan Template
- Last known-good release/version:
- Rollback trigger conditions:
- Rollback owner:
- Recovery steps:
- Validation checks after rollback:

## Communications Plan Template
- Audience(s):
- Channel(s):
- Pre-release notice timing:
- Release start update:
- Release completion update:
- Incident/escalation contact path:

## Post-deploy Verification
- [ ] Smoke tests complete
- [ ] Key business flows verified
- [ ] Error rates and latency within expected range
- [ ] No active Sev-1/Sev-2 issues introduced
- [ ] Release summary posted with next actions (if any)
