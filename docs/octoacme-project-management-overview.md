# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
Every project draws from the following team members (not all required for every project):

### Always Present
- **Project Manager (PM)**: coordinates delivery, schedules, risk, communications.
- **Product Manager (PdM)**: defines outcomes, prioritizes backlog, and measures success.
- **Developers**: implement features, collaborate on design and testability.

### Typically Involved
- **QA Lead**: defines quality standards, test strategy, and sign-off for feature acceptance.
- **Release Manager**: coordinates release planning and deployment.
- **DevOps Engineer**: builds and maintains CI/CD pipelines and deployment infrastructure.
- **UX Designer**: ensures user-centered design and accessibility.
- **Technical Writer**: documents processes, features, and changes.

See **octoacme-roles-and-personas.md** for detailed descriptions of responsibilities and collaboration patterns.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items
- Release Notes and Change Log
- Process Documentation

## Lifecycle (high-level)
1. **Initiation**: problem statement, stakeholders, high-level timeline.
2. **Planning**: scope, resources, milestones, dependencies, quality gates, and test strategy.
3. **Execution**: build, test, review, iterate.
4. **Release**: deploy, verify, announce.
5. **Close & Retrospective**: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Pre-release coordination and release announcements (Release Manager)
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
- Reference the personas in `octoacme-roles-and-personas.md` to ensure cross-functional clarity.
