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

### Testing Strategy
- **QA Lead** defines and documents the test strategy at project kickoff
- Quality gates are established: when automated tests suffice vs. when manual testing is required
- Testing occurs at multiple levels:

### Test Coverage
- Unit tests for new logic (owned by Developers)
- Integration tests where applicable (owned by Developers or QA)
- End-to-end smoke tests for critical flows before release (owned by QA Lead)
- Security scanning in CI (automated, DevOps or security team)

### Feature Acceptance
- QA Lead reviews acceptance criteria with Product Managers and Developers during planning
- Manual QA for feature acceptance when needed (QA Lead leads, Developers support)
- QA Lead signs off on feature readiness before moving to release phase

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)
- QA Lead tracks test coverage and defect escape rates

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Test strategy and quality gates documented (QA Lead)
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] QA Lead sign-off process defined for feature acceptance
