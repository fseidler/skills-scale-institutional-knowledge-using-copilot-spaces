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
- Use a single source of truth (project README or release doc) for status

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
- Level 1: Team-level triage and resolution (1-3 days)
- Level 2: PM escalates to Product Lead and dependent teams (3-7 days)
- Level 3: Sponsor-level escalation for business-impacting issues (1-3 days for decision)
- Level 4: Executive/Incident response for critical production or security issues (immediate)

For detailed escalation procedures, criteria, and communication templates, see the [Risk Escalation Paths Guide](templates/risk-escalation-paths.md).

**Security Incidents:** Follow the security incident runbook and notify Security on-call immediately. Reference Level 4 escalation in the Risk Escalation Paths Guide.
