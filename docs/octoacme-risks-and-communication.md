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

### Weekly Status Update Template
**Project:** [Project Name]  
**Week ending:** [Date]  
**Status:** 🟢 On Track / 🟡 At Risk / 🔴 Blocked

**Progress this week:**
- [Key milestone or deliverable completed]
- [Features shipped or PRs merged]
- [Important decisions made]

**Next steps:**
- [Planned work for next week]
- [Upcoming milestones]

**Risks & blockers:**
- [Current risks with severity: High/Med/Low]
- [Active blockers and mitigation plans]
- [Dependencies waiting on other teams]

**Ask / decisions needed:**
- [Specific decisions required from stakeholders]
- [Resources or support needed]

**Metrics snapshot (if applicable):**
- Velocity: [completed story points or tasks]
- Burndown: [on/ahead/behind schedule]
- Quality: [bug count, test coverage]

---

### Risk Communication Template
**Risk ID:** [Unique identifier]  
**Date identified:** [Date]  
**Status:** Open / Mitigated / Closed

**Description:**
[Clear description of the risk]

**Impact:** High / Medium / Low  
[Describe the potential impact on scope, schedule, quality, or cost]

**Likelihood:** High / Medium / Low  
[Estimate probability of occurrence]

**Category:** Technical / Resource / Schedule / External / Compliance

**Owner:** [Person responsible for monitoring and mitigation]

**Mitigation plan:**
- [Action 1 to reduce likelihood or impact]
- [Action 2]
- [Contingency plan if risk materializes]

**Status updates:**
- [Date]: [Update on mitigation progress]
- [Date]: [Update on mitigation progress]

---

### Incident Communication Template
**Incident:** [Brief title]  
**Severity:** Critical / High / Medium / Low  
**Status:** Investigating / Identified / Mitigating / Resolved  
**Started:** [Date/Time]

**Triage summary:**
[What happened, what is affected, initial assessment]

**Impact:**
- Users affected: [scope of impact]
- Features/services impacted: [list]
- Business impact: [if applicable]

**Actions being taken:**
1. [Current action]
2. [Next step]

**Expected timeline:**
- Mitigation ETA: [time]
- Full resolution ETA: [time]

**Stakeholder notifications:**
- [Who has been notified]
- [Communication channels being used]

**Next update:** [Time for next status update]

**Post-incident:**
- Blameless retrospective scheduled: [Date/Time]
- Root cause analysis owner: [Person]

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

### Escalation by Persona
- **Developers:** Technical blocker → Tech Lead → Project Manager → Product Lead
- **UX Designer:** Design conflict or user experience risk → Product Manager → Product Lead
- **QA Lead:** Release blocker or quality risk → Project Manager + Product Manager → Product Lead
- **Customer Support:** Critical customer issue → Product Manager + Project Manager (if systemic)
- **Business Analyst:** Requirements conflict or stakeholder misalignment → Product Manager + Project Manager → Sponsor

---

_Related: Enhanced templates address gaps identified in [issue #4](https://github.com/edudelpozo/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._
