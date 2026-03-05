# OctoAcme — RACI & Ownership

## Purpose
Provide a lightweight RACI matrix for core project lifecycle activities so every team member knows who is Responsible, Accountable, Consulted, and Informed for each phase.

## RACI Key
| Letter | Meaning |
|--------|---------|
| **R** | **Responsible** — Does the work |
| **A** | **Accountable** — Owns the outcome (only one per row) |
| **C** | **Consulted** — Provides input before/during |
| **I** | **Informed** — Notified of progress/outcome |

## RACI Matrix

| Activity | PM | PdM | Dev Lead | Developer | QA | Security | Stakeholders |
|----------|----|----|----------|-----------|----|----------|--------------|
| Project initiation & charter | A/R | C | C | I | I | I | C |
| Backlog creation & prioritization | C | A/R | C | C | C | I | C |
| Sprint / iteration planning | A/R | C | R | R | C | I | I |
| Execution & daily tracking | A/R | I | R | R | R | I | I |
| Risk identification & mitigation | A/R | C | C | C | C | C | I |
| Release readiness review | A/R | C | C | R | R | C | I |
| Deployment & rollback decisions | C | I | A/R | R | C | C | I |
| Incident response | R | I | A/R | R | R | R | I |
| Retrospective facilitation | A/R | C | C | R | R | I | I |
| Decision log maintenance | A/R | C | C | I | I | I | I |

> **Note:** "A/R" means a single person is both Accountable and responsible for doing the work. Adjust per team structure.

## Directly Responsible Individual (DRI)

### Definition
The **DRI** is the single person who owns a deliverable or decision and is ultimately answerable for its outcome. There can only be one DRI per item.

### DRI vs. Accountable (RACI)
The DRI maps to the **Accountable** role in the RACI matrix. When in doubt, the DRI is the person who would be called on to explain the status or rationale of the item.

### Using DRI with GitHub Issues & Projects
1. **Assign the issue** to the DRI in GitHub Issues — one assignee per decision or deliverable issue.
2. **Label appropriately** — use labels like `dri:<name>` or a custom field in GitHub Projects for visibility.
3. **Reference in PR descriptions** — include `DRI: @username` in the PR template so reviewers know who to contact.
4. **Decision Log** — every decision entry in the [Decision Log](octoacme-decision-log.md) must name a DRI in the Owner/DRI column.

## How to Use This Document
- At project kickoff, fill in the names (not just roles) in a project-specific copy of the matrix.
- Review and update the matrix when team membership or responsibilities change.
- Reference this doc during planning and retros to clarify ownership disputes.
