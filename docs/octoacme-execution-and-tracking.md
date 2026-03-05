# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- All items must meet the [Definition of Done](octoacme-definition-of-ready-and-done.md) before being marked complete

## Handoff to QA / Release Gate
Before moving a work item to the **QA** or **Done** column:
1. Confirm all [Definition of Done](octoacme-definition-of-ready-and-done.md) criteria are met.
2. Assign a QA reviewer and link the relevant PR or build.
3. For release-bound items, confirm a [Release Readiness Checklist](octoacme-release-readiness-checklist.md) has been started.

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

### Escalation Triggers & Response Times
| Trigger | Expected Response Time |
|---------|----------------------|
| Item blocked > 2 business days | Escalate to Level 2 within 24 hours |
| Milestone slip risk identified | PM to assess and notify stakeholders same day |
| Production incident affecting customers | Immediately trigger incident comms — see [Risk Management & Communication](octoacme-risks-and-communication.md) |

> For the full escalation trigger list including security, privacy, and third-party dependency scenarios, see [Risk Management & Communication](octoacme-risks-and-communication.md).

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
