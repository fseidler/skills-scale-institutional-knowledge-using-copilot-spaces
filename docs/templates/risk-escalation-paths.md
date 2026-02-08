# Risk Escalation Paths and Procedures

**Version:** 1.0  
**Last Updated:** 2026-02-08  
**Purpose:** Define clear escalation paths for risks, issues, and blockers to ensure rapid resolution

## Overview

Effective risk escalation ensures that problems are addressed at the appropriate level with the right urgency. This document outlines escalation paths, criteria for escalation, and response expectations for different types of risks.

---

## Escalation Levels

### Level 1: Team-Level Resolution
**When to use:** Minor risks, blockers that can be resolved within the immediate team

**Examples:**
- Technical dependency on another team member
- Clarification needed on requirements
- Small scope questions
- Minor tool or access issues

**Process:**
1. Raise in daily standup
2. Team discusses and identifies owner
3. Owner commits to resolution timeline
4. Follow up in next standup if unresolved

**Expected Resolution Time:** 1-3 days  
**Decision Authority:** Team Lead, Senior Developer, or assigned owner

---

### Level 2: Project Manager Escalation
**When to use:** Issues requiring cross-team coordination, resource allocation, or schedule adjustments

**Examples:**
- External team dependency causing delays
- Resource constraints impacting timeline
- Medium-priority technical risks
- Scope clarification needed from Product Manager
- Testing or environment issues blocking progress

**Process:**
1. Team member or lead raises to Project Manager
2. PM assesses impact and urgency
3. PM coordinates with relevant parties (Product Manager, other teams, stakeholders)
4. PM updates risk register and communicates resolution plan
5. PM tracks to completion and reports in weekly status

**Expected Resolution Time:** 3-7 days  
**Decision Authority:** Project Manager, with input from Product Manager

---

### Level 3: Product Lead / Sponsor Escalation
**When to use:** High-impact risks requiring executive decision-making, significant resources, or strategic tradeoffs

**Examples:**
- Project timeline in jeopardy (>2 week delay)
- Major scope changes needed
- Critical resource unavailability
- Dependency on another project causing significant risk
- Budget overrun concerns
- High-severity security vulnerabilities requiring immediate action
- Regulatory or compliance issues

**Process:**
1. Project Manager escalates to Product Lead/Sponsor with:
   - Clear problem statement
   - Impact assessment (timeline, scope, quality, budget)
   - Options analysis with pros/cons
   - Recommended course of action
2. Product Lead/Sponsor convenes decision meeting if needed
3. Decision made and communicated to all stakeholders
4. PM updates project plan and risk register
5. PM communicates plan to team and monitors execution

**Expected Resolution Time:** 1-3 days for decision; implementation varies  
**Decision Authority:** Product Lead, Executive Sponsor, or steering committee

---

### Level 4: Executive / Incident Response Escalation
**When to use:** Critical production issues, security incidents, or business-threatening risks

**Examples:**
- Production outage or critical system failure
- Data breach or security incident
- Regulatory violation discovered
- Legal or compliance emergency
- Critical customer escalation
- Reputational risk

**Process:**
1. Immediate notification via defined incident channels (on-call, Slack, email)
2. Incident commander assigned
3. War room or incident bridge activated
4. Executive stakeholders notified
5. Follow incident response playbook
6. Regular status updates until resolution
7. Post-incident review scheduled

**Expected Response Time:** Immediate (15-30 minutes)  
**Decision Authority:** Incident Commander, CTO, CEO (depending on severity)

---

## Risk Type-Specific Escalation Paths

### Technical Risks

| Risk Category | Level 1 | Level 2 | Level 3 | Level 4 |
|--------------|---------|---------|---------|---------|
| Architecture/Design | Team Lead | PM + Tech Lead | Product Lead + CTO | CTO + CEO |
| Performance Issues | Developer | PM + Tech Lead | Product Lead | Incident Commander |
| Third-party Dependencies | Developer | PM | Product Lead | Product Lead + Legal |
| Technical Debt | Team Lead | PM + Product Manager | Product Lead | N/A |

### Security Risks

| Risk Category | Level 1 | Level 2 | Level 3 | Level 4 |
|--------------|---------|---------|---------|---------|
| Code Vulnerabilities | Developer | Security Lead + PM | Security Lead + CTO | CISO + CEO |
| Security Incident | N/A | Security Lead | CISO | CISO + CEO + Legal |
| Compliance Issues | Security Lead | Security Lead + PM | CISO + Legal | CISO + CEO + Legal |
| Data Privacy Concerns | Security Lead | Security Lead + PM | CISO + Legal | CISO + CEO + Legal |

### Process/People Risks

| Risk Category | Level 1 | Level 2 | Level 3 | Level 4 |
|--------------|---------|---------|---------|---------|
| Resource Constraints | Team Lead | PM | Product Lead + Sponsor | Executive Team |
| Team Conflicts | Team Members | PM + Manager | HR + Senior Management | HR + Executive Team |
| Communication Gaps | Team Lead | PM | Product Lead | Product Lead + Stakeholders |
| Dependency Delays | Team Lead | PM | Product Lead | Product Lead + Dependent Execs |

### Business Risks

| Risk Category | Level 1 | Level 2 | Level 3 | Level 4 |
|--------------|---------|---------|---------|---------|
| Scope Changes | Product Manager | PM + Product Manager | Product Lead + Sponsor | Executive Steering Committee |
| Budget Overruns | PM | PM + Product Lead | Product Lead + Finance | CFO + Executive Team |
| Timeline Delays | PM | PM + Product Lead | Product Lead + Sponsor | Executive Steering Committee |
| Market/Competitive | Product Manager | Product Lead | Product Lead + CEO | Executive Team |

---

## Escalation Best Practices

### Before Escalating
1. **Gather Facts:** Collect all relevant information, data, and context
2. **Assess Impact:** Quantify the impact on timeline, scope, quality, and budget
3. **Propose Solutions:** Identify possible solutions and their tradeoffs
4. **Document:** Update risk register with current status and proposed escalation

### When Escalating
1. **Be Clear:** State the problem, impact, and urgency concisely
2. **Be Timely:** Don't wait until it's too late to course-correct
3. **Be Solution-Oriented:** Present options, not just problems
4. **Be Transparent:** Share all relevant facts, even if uncomfortable

### After Escalating
1. **Follow Through:** Execute the decision promptly
2. **Communicate:** Update all relevant stakeholders on the outcome
3. **Document:** Record the decision and rationale in the risk register
4. **Learn:** Capture lessons learned for future retrospectives

---

## Communication Templates

### Level 2 Escalation Email Template

**Subject:** [Project Name] - Risk Escalation: [Brief Description]

**Priority:** High / Medium  
**Impact:** Timeline / Scope / Quality / Budget / All

**Problem Statement:**
[Clear, concise description of the issue]

**Current Status:**
[What's been tried, current state]

**Impact Assessment:**
- Timeline: [Impact on schedule]
- Scope: [Impact on deliverables]
- Quality: [Impact on quality metrics]
- Resources: [Impact on team/budget]

**Options:**
1. [Option 1: Pros/Cons]
2. [Option 2: Pros/Cons]
3. [Option 3: Pros/Cons]

**Recommendation:**
[Recommended course of action with rationale]

**Next Steps:**
[Immediate actions needed]

**Decision Needed By:**
[Date/Time]

---

### Level 3 Escalation Briefing Template

**Project:** [Name]  
**Date:** [Date]  
**Escalated By:** [Name, Role]  
**Urgency:** High / Critical

**1. Executive Summary (2-3 sentences)**
[What happened, why it matters, what decision is needed]

**2. Background**
[Context needed to understand the situation]

**3. Problem Statement**
[Clear articulation of the core issue]

**4. Impact Analysis**
| Category | Without Action | With Option A | With Option B |
|----------|---------------|---------------|---------------|
| Timeline | [Impact] | [Impact] | [Impact] |
| Budget | [Impact] | [Impact] | [Impact] |
| Scope | [Impact] | [Impact] | [Impact] |
| Risk | [Impact] | [Impact] | [Impact] |

**5. Options Analysis**
- **Option A:** [Description, pros, cons, cost]
- **Option B:** [Description, pros, cons, cost]
- **Option C:** [Description, pros, cons, cost]

**6. Recommendation**
[Clear recommendation with rationale]

**7. Decision Required**
[Specific decision or approval needed]

**8. Timeline**
- Decision needed by: [Date]
- Implementation start: [Date]
- Expected resolution: [Date]

---

## Monitoring and Review

- **Risk Register Updates:** All escalations must be documented in the risk register
- **Weekly Review:** PM reviews all active escalations in weekly status meetings
- **Monthly Metrics:** Track escalation frequency, resolution time, and outcomes
- **Retrospective Analysis:** Review escalation effectiveness in sprint/project retrospectives

---

## Roles and Responsibilities

| Role | Escalation Responsibility |
|------|--------------------------|
| **Team Members** | Identify and raise risks early; provide context and input |
| **Team Lead** | Triage Level 1 risks; escalate to PM when needed |
| **Project Manager** | Own escalation process; coordinate Level 2 and Level 3 escalations |
| **Product Manager** | Provide business context; make scope/priority decisions |
| **Product Lead** | Make strategic tradeoff decisions; approve major changes |
| **Security Lead** | Triage and escalate security risks; activate incident response |
| **Sponsor** | Provide executive decision-making; allocate resources |

---

## Appendix: Contact Information

### Emergency Contacts
- **Incident Commander On-Call:** [Contact]
- **Security On-Call:** [Contact]
- **IT Support:** [Contact]
- **Executive Sponsor:** [Contact]

### Escalation Channels
- **Level 1-2:** Slack: #project-[name], Email: [DL]
- **Level 3:** Email: [Executive DL], Slack: #leadership
- **Level 4:** Phone/SMS: [On-call numbers], Incident Bridge: [Link]

---

**Note:** This template should be customized for each project with specific contact information, communication channels, and decision-makers. Review and update escalation paths at project kickoff and whenever team structure changes.
