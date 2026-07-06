# Release Manager — Checklist

Purpose: A checklist for Release Managers to ensure consistent, safe, and well-communicated releases.

Before release (planning)
- [ ] Confirm release scope and included PRs/issues
- [ ] Confirm all feature owners and QA owners identified
- [ ] Validate that the release branch has passed CI, security scans, and automated tests
- [ ] Confirm smoke tests and post-deploy checks are defined
- [ ] Confirm rollback plan and previous good release point
- [ ] Confirm maintenance window and stakeholder notification schedule
- [ ] Confirm Support Liaison is prepared with KB/playbooks

Staging
- [ ] Deploy to staging and run smoke tests
- [ ] Run performance and quick acceptance checks for critical paths
- [ ] Validate observability: dashboards and alerts for key metrics
- [ ] Conduct sign-off with PM, QA, Platform

Production deploy
- [ ] Start deployment in scheduled window
- [ ] Monitor deployment progress and health metrics
- [ ] Run smoke tests in production
- [ ] Confirm rollback criteria and be ready to execute if needed
- [ ] Notify stakeholders when deployment completes or if rollback occurs

Post-deploy
- [ ] Validate success metrics (initial telemetry checks)
- [ ] Confirm customer-facing release notes are published
- [ ] Ensure support runbooks and KB articles are accessible
- [ ] Capture any deployment issues into backlog and assign owners
- [ ] Short retro: Was deployment successful? Action items?

Notes:
- For emergency/patch releases, follow the incident runbook and coordinate with on-call and Security if relevant.
