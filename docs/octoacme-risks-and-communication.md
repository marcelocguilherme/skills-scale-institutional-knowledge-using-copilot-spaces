# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use the [Project Status Page](octoacme-project-status-template.md) as the single source of truth for project status; update it at least weekly or after each milestone
- Share the status page link in all stakeholder communications rather than duplicating content

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

### Escalation Triggers & Response Times
| Trigger | Expected Response Time |
|---------|----------------------|
| Item blocked > 2 business days | PM escalates to Level 2 within 24 hours |
| Milestone slip risk identified | PM assesses and notifies stakeholders same day |
| Security or privacy risk discovered | Escalate to Security on-call immediately |
| Production incident affecting customers | Trigger incident comms template (below) immediately |
| Third-party dependency failure | PM escalates to vendor contact and Product Lead within 4 hours |

> For execution-level escalation triggers also see [Execution & Tracking](octoacme-execution-and-tracking.md).
