# OctoAcme — Quality Gates and Test Strategy

## Purpose
Define practical quality gates and ownership so teams can make consistent, low-ambiguity release decisions.

## Stage-based Quality Gates

### In Review
- **Goal:** ensure changes are implementation-ready before QA
- **Required checks**
  - PR includes issue link and acceptance criteria
  - Automated tests for changed behavior are present and passing
  - Peer review approval captured
- **Primary ownership**
  - **Developers (R):** code quality, tests, and PR completeness
  - **QA Lead (C):** testability and edge-case consultation
  - **PM/PdM (C):** acceptance criteria clarity and scope alignment

### QA
- **Goal:** validate behavior against acceptance criteria and risk profile
- **Required checks**
  - Test cases executed for feature, regression, and critical paths
  - Defects triaged with severity and release impact
  - Exit criteria documented by QA Lead
- **Primary ownership**
  - **QA Lead (A/R):** QA execution strategy and quality decision
  - **Developers (R):** defect resolution and retest support
  - **PM/PdM (C):** scope trade-offs and release-risk decisions

### Pre-release
- **Goal:** ensure production readiness from quality and operational perspectives
- **Required checks**
  - QA gate passed and unresolved defects have explicit disposition
  - Smoke-test plan verified for post-deploy
  - Rollback and communication plans are ready
- **Primary ownership**
  - **Release Manager (A):** go/no-go facilitation
  - **QA Lead (R):** quality confidence statement
  - **DevOps Engineer (R):** deployment/monitoring readiness
  - **PM/PdM (C):** customer-impact acceptance and stakeholder alignment

## Defect Triage Guidelines
- **Critical (Sev-1):** blocks release unless explicit executive exception
- **High (Sev-2):** requires mitigation plan and owner before release
- **Medium/Low:** may be deferred with documented rationale and target iteration

## Minimal Evidence to Record Per Release
- Link to QA summary and open-defect disposition
- Quality gate decisions and approver names
- Post-deploy verification results
- Follow-up actions with owners and due dates
