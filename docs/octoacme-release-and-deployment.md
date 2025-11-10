# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## QA Pre-Release Checklist

### Testing Validation
- [ ] All planned test cases executed and passed
- [ ] Automated test suite passing (unit, integration, E2E)
- [ ] Manual exploratory testing completed for new features
- [ ] Regression testing completed for affected areas
- [ ] Performance testing completed (if applicable)
- [ ] Security scanning passed (no critical/high vulnerabilities)
- [ ] Accessibility testing completed (if user-facing)
- [ ] Cross-browser/device testing completed (if applicable)

### Bug & Issue Review
- [ ] All critical and high-priority bugs resolved
- [ ] Medium-priority bugs triaged (fix, defer, or document as known issue)
- [ ] Known issues documented in release notes
- [ ] No open P0/P1 bugs blocking release

### Documentation & Communication
- [ ] Test results documented and shared with team
- [ ] QA sign-off obtained
- [ ] Customer Support informed of changes and known issues
- [ ] User documentation updated (if applicable)
- [ ] API documentation updated (if applicable)

### Environment Readiness
- [ ] Staging environment mirrors production configuration
- [ ] Test data prepared and validated
- [ ] Third-party integrations tested in staging
- [ ] Database migrations tested (if applicable)

## Deployment Checklist

### Pre-Deployment
- [ ] Deployment window scheduled (if needed)
- [ ] Stakeholders notified of deployment schedule
- [ ] Deployment team assigned and available
- [ ] Backup or snapshot created (if applicable)
- [ ] Rollback plan documented and tested
- [ ] Monitoring and alerting configured

### Staging Deployment
- [ ] Deploy to staging environment
- [ ] Run automated smoke tests
- [ ] QA Lead validates critical paths
- [ ] UX Designer reviews UI changes (if applicable)
- [ ] Performance metrics within acceptable range

### Production Deployment
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Monitor deployment progress and logs
- [ ] Run post-deploy verification tests
- [ ] Validate key metrics and health checks
- [ ] Confirm no errors in application logs

### Post-Deployment
- [ ] Announce release to stakeholders and Customer Support
- [ ] Update status page (if applicable)
- [ ] Monitor for first 30-60 minutes post-release
- [ ] Verify success metrics and user feedback
- [ ] Document any issues encountered during deployment
- [ ] Close release tracking issue/ticket

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

---

_Related: Enhanced checklists address gaps identified in [issue #4](https://github.com/edudelpozo/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._
