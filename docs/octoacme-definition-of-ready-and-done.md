# OctoAcme — Definition of Ready & Definition of Done

## Purpose
Provide standard checklists that ensure backlog items are well-formed before being pulled into a sprint (DoR) and that completed work genuinely meets quality and release standards before being marked Done (DoD).

## Definition of Ready (DoR)
A backlog item is **Ready** when all of the following are true:

- [ ] Problem statement or user story is written and understood by the team
- [ ] Acceptance criteria (AC) are defined, specific, and testable
- [ ] Dependencies (internal and external) are identified and unblocked, or a plan exists to unblock them
- [ ] Design notes, wireframes, or technical spike results are available (if required)
- [ ] Test approach is outlined (unit, integration, manual QA, etc.)
- [ ] Telemetry / observability impact is considered (new metrics, logging, dashboards)
- [ ] Rollout strategy or feature flag plan is noted (if applicable)
- [ ] Item is estimated (story points or T-shirt size)
- [ ] Item is prioritized in the backlog relative to other items

> **When to apply:** Review this checklist during backlog refinement and at the start of sprint planning. Items that do not meet DoR should not be pulled into the sprint.

## Definition of Done (DoD)
A backlog item is **Done** when all of the following are true:

- [ ] All acceptance criteria are met and verified
- [ ] Automated tests (unit, integration) written and passing in CI
- [ ] Documentation updated (inline comments, README, relevant process docs)
- [ ] Security and dependency scans passing in CI
- [ ] Observability confirmed: new metrics/logs are in place and dashboards updated if needed
- [ ] Feature flag or rollout plan executed per agreed strategy
- [ ] Release notes entry drafted (for user-facing or breaking changes)
- [ ] PR reviewed and approved per team policy
- [ ] QA sign-off obtained (manual or automated, as agreed per item)
- [ ] No known P0/P1 defects introduced

> **When to apply:** Check this list before moving a card to **Done** on the project board and before handing off to QA or release. See [Execution & Tracking](octoacme-execution-and-tracking.md) for the handoff gate guidance.

## Customizing These Checklists
- Teams may add project-specific items but should not remove items without team agreement.
- Record any customisations in the project README or project charter.
- Review and update the checklists during retrospectives as the process matures. See [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).
