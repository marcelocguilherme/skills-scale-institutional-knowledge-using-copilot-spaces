# OctoAcme — Decision Log

## Purpose
Record significant project decisions so the team has a single reference for what was decided, why, and by whom. Use this log to avoid re-litigating past decisions and to provide context in retros or post-mortems.

## When to Use
- Any decision that affects scope, architecture, schedule, or process
- When multiple options were considered and a rationale needs to be preserved
- When a decision requires explicit approval from a stakeholder or sponsor
- When a decision is likely to be revisited or queried later

## Decision Log Table

| # | Date | Decision | Context / Problem | Options Considered | Owner / DRI | Approver(s) | Impacted Areas | Links |
|---|------|----------|-------------------|--------------------|-------------|-------------|----------------|-------|
| 1 | YYYY-MM-DD | _Short statement of what was decided_ | _Why a decision was needed_ | _Option A, Option B, …_ | @username | @username | e.g., API, infra | Issue / PR / Doc |

> **Tip:** Keep decisions concise. Link to longer design docs, RFCs, or ADRs for detailed analysis.

## How to Add an Entry
1. Assign the next sequential number.
2. Fill in all columns — leave none blank; use "N/A" if not applicable.
3. Paste the issue or PR link in the **Links** column so the decision is traceable.
4. Notify impacted team members when a new entry is added.

## Linking Decisions to Issues, PRs, and Retros
- **Issues / PRs:** Reference the decision number in the issue or PR description (e.g., `Decision #3 in decision log`).
- **Retrospectives:** Review open or recently-made decisions as part of the retro to confirm they are still valid and capture any follow-on action items. See [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).
- **DRI Ownership:** Each decision must have a named DRI (Directly Responsible Individual). See [RACI & Ownership](octoacme-raci-and-ownership.md) for guidance.

## Tips for Good Decision Logging
- Log decisions *at the time they are made*, not retroactively.
- If a decision is reversed, add a new entry rather than editing the old one.
- Archive old logs at the end of a project phase but keep them accessible.
