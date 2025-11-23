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

### Risk Register Template

| ID | Description | Impact | Likelihood | Owner | Mitigation Plan | Status |
|----|-------------|--------|------------|-------|----------------|--------|
| R-001 | Example: Key developer unavailable | High | Low | PM | Cross-train team members; document critical knowledge | Open |
| R-002 | Example: Third-party API instability | Med | Med | Solution Architect | Implement retry logic and fallback mechanism | Mitigated |
| R-003 | Example: Unclear requirements | High | Med | Business Analyst | Conduct stakeholder workshops; create detailed acceptance criteria | Closed |

**Risk Severity Matrix**: Combine Impact × Likelihood to prioritize
- **Critical (High/High)**: Immediate escalation and mitigation required
- **High (High/Med or Med/High)**: Active monitoring and mitigation plan needed
- **Medium (Med/Med, High/Low, Low/High)**: Regular review and contingency planning
- **Low (Low/Low, Low/Med, Med/Low)**: Monitor and accept

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

### Stakeholder Communication Plan Template

| Stakeholder Group | Communication Need | Frequency | Format | Owner | Example Topics |
|-------------------|-------------------|-----------|--------|-------|----------------|
| Executive Sponsors | High-level progress, risks, decisions | Monthly | Email summary or slide deck | Project Manager | Milestone status, budget, major risks |
| Product Leadership | Feature delivery, roadmap alignment | Bi-weekly | Sync meeting | Product Manager | Backlog priorities, user feedback |
| Engineering Teams | Technical details, dependencies | Weekly | Standup + Slack updates | Tech Lead / Solution Architect | API changes, integration points |
| Support Team | New features, known issues, FAQs | Per release | Documentation + training session | Product Manager | Feature guides, troubleshooting tips |
| End Users | Feature announcements, release notes | Per release | Email + in-app notifications | Product Manager | What's new, how-to guides |

**Best Practices**:
- Tailor message detail to audience needs
- Use consistent format and schedule for predictability
- Highlight action items and decisions clearly
- Escalate blockers proactively, not reactively

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
