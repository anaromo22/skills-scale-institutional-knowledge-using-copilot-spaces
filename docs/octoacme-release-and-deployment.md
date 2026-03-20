# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Manager Role
The **Release Manager** coordinates all release activities and serves as the single point of accountability for deployment success. The Release Manager:
- Schedules the release and communicates timelines to all stakeholders
- Verifies completion of all pre-release requirements
- Manages release notes and stakeholder communications
- Coordinates with DevOps on deployment scheduling and monitoring
- Leads incident response if issues arise during or after deployment

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release Requirements
- All acceptance criteria met and PRs merged
- QA Lead has signed off on feature readiness
- Passing CI and security scans
- Release notes drafted (by Technical Writer or Product Manager)
- Rollback / mitigation plan documented (by DevOps and Release Manager)
- Smoke tests prepared (by QA Lead)

## Pre-Release Coordination (Release Manager owns)
1. **Notify stakeholders** 2–3 weeks before planned release
2. **Lock the release branch** (no new commits except critical fixes)
3. **Verify all pre-release requirements** with engineering and QA
4. **Prepare release notes** with Technical Writer
5. **Schedule deployment window** with DevOps and on-call team
6. **Brief support team** on new features and known issues

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] DevOps deploys to staging and QA runs smoke tests
- [ ] Release Manager clears deployment (all checks passed)
- [ ] DevOps deploys to production (automated pipeline preferred)
- [ ] Post-deploy verification: DevOps and QA run checks in real-time
- [ ] Release Manager announces release to customers and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Release Manager triggers incident response and notifies on-call
  - DevOps evaluates rollback necessity
  - If rollback is needed, execute and return to last known-good release
  - Triage root cause in post-incident retrospective and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
- Support contact / escalation path:

## Post-Release Activities
- Release Manager ensures monitoring dashboards are active
- QA Lead monitors for defects in production
- Technical Writer updates documentation if needed
- Team conducts release retrospective within 1 week (see Retrospective & Continuous Improvement)
