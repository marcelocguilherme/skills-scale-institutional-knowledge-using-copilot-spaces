# OctoAcme — Release Readiness Checklist

## Purpose
Provide a structured readiness review gate before any release is approved. Use this checklist to confirm that the team has addressed quality, security, rollout, and communication requirements, and to capture explicit sign-offs from required approvers.

## When to Use
Complete this checklist during the **release readiness review** meeting (or async review for low-risk patches) before promoting a build to production. See [Release & Deployment Guide](octoacme-release-and-deployment.md) for the broader deployment process.

---

## Readiness Review Checklist

### Functionality & Quality
- [ ] All acceptance criteria met for items included in this release
- [ ] All automated tests (unit, integration, end-to-end smoke) passing in CI
- [ ] No open P0 or P1 defects in scope for this release
- [ ] Manual QA sign-off obtained for user-facing changes
- [ ] Regression suite executed and results reviewed

### Security & Compliance
- [ ] Security scans (SAST, dependency scanning) passing with no new critical/high findings
- [ ] Privacy review completed if personal data handling changed
- [ ] Secrets/credentials not hardcoded; vault/config management verified
- [ ] Compliance or regulatory requirements reviewed (if applicable)

### Observability & Reliability
- [ ] Monitoring and alerting configured for new or changed components
- [ ] Dashboards updated to reflect new metrics or log streams
- [ ] Runbook or playbook updated for any new failure modes
- [ ] SLO / SLA impact assessed

### Rollout & Feature Flags
- [ ] Feature flag configuration reviewed and set correctly for target rollout percentage
- [ ] Staged rollout plan documented (e.g., 1% → 10% → 100%)
- [ ] Rollback procedure tested or confirmed (e.g., flag disable, prior artifact available)

### Release Communication
- [ ] Release notes drafted and reviewed
- [ ] Stakeholders and support team notified of upcoming release
- [ ] Known issues documented in release notes
- [ ] Post-release monitoring window agreed (e.g., 24–48 hours of heightened watch)

---

## Sign-offs

| Role | Name | Date | Signature / Approval link |
|------|------|------|---------------------------|
| DRI / Project Manager | | YYYY-MM-DD | |
| QA Lead | | YYYY-MM-DD | |
| Product Manager | | YYYY-MM-DD | |
| Security (if required) | | YYYY-MM-DD | |

> **All required sign-offs must be recorded before the deployment is triggered.**  
> For patch releases, a single DRI sign-off with noted exceptions is acceptable; document the exception reason in the Decision Log. See [Decision Log](octoacme-decision-log.md).

---

## After the Release
- Update the [Project Status Page](octoacme-project-status-template.md) to reflect the release milestone.
- File a retrospective action item for any checklist items that were waived or problematic.
