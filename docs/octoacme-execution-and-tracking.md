# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - Participants: Developers, Project Manager, QA Lead (as needed)
- Weekly delivery sync — show progress, updates, and flagged risks
  - Participants: Project Manager, Product Manager, Developers, UX Designer, QA Lead
- Demo/Review at the end of each sprint or milestone
  - Participants: Full delivery team, stakeholders, Customer Support (for user-facing features)
- Design reviews (as needed) — UX Designer presents designs for feedback
  - Participants: UX Designer, Product Manager, Developers, QA Lead
- Requirements refinement (as needed) — clarify upcoming work
  - Participants: Business Analyst, Product Manager, Project Manager, Tech Lead

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

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

### Persona-Specific Escalation Examples
- **Quality Issues:** QA Lead identifies release blocker → Project Manager + Product Manager → Go/no-go decision
- **Design Concerns:** UX Designer raises usability risk → Product Manager → Design review with stakeholders
- **Customer Impact:** Customer Support reports systemic issue → Product Manager triages → Incident response if needed
- **Requirements Gaps:** Business Analyst surfaces requirement conflict → Product Manager + stakeholders → Requirements alignment session

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

---

_Related: Meeting rhythms updated to include new personas from [issue #4](https://github.com/edudelpozo/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._
