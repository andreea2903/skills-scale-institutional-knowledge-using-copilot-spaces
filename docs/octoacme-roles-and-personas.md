# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Additional Personas (new additions)

These specialized personas address cross-cutting concerns that improve clarity of ownership, release safety, observability, accessibility, and customer-facing support.

### Release Manager
- Responsibilities:
  - Owns release planning and execution across staging and production.
  - Coordinates deployment windows, rollback strategies, and release communications.
  - Ensures release readiness criteria are met (merged PRs, passing CI, smoke tests, migration steps, release notes).
- Interactions:
  - Works closely with PM, Platform/DevOps, QA, and Support Liaison to schedule and validate releases.
  - Notifies stakeholders, on-call, and support teams before and after releases.
- When to involve:
  - At release planning, when deployment risks are identified, and during post-deploy verification.

### Platform / DevOps Engineer
- Responsibilities:
  - Maintains CI/CD pipelines, infrastructure as code, and deployment automation.
  - Owns monitoring, alerting, runbooks, and operational reliability improvements.
  - Implements platform-level changes and ensures secure configurations.
- Interactions:
  - Implements requests from Developers and Release Manager.
  - Partners with Security for hardening and with Data Analysts for observability dashboards.
- When to involve:
  - For pipeline or infra changes, deployment issues, and runbook updates.

### UX Researcher / Designer
- Responsibilities:
  - Conducts user research and usability testing; provides design guidance and prototypes.
  - Ensures designs meet usability and accessibility standards.
- Interactions:
  - Works with Product Managers to inform requirements and acceptance criteria.
  - Collaborates with Developers and QA to validate UX and accessibility acceptance criteria.
- When to involve:
  - Early in planning, before finalizing significant UX or flow decisions.

### Data Analyst / Insights Owner
- Responsibilities:
  - Defines and validates success metrics and required instrumentation.
  - Implements tracking plans or coordinates telemetry work and analyses outcomes.
- Interactions:
  - Works with Product Managers to set success metrics and with Developers to implement telemetry.
  - Produces reports for PMs and stakeholders post-release.
- When to involve:
  - During planning to define measurable outcomes and to validate instrumented data before release.

### Support Liaison / Customer Ops
- Responsibilities:
  - Serves as the primary contact for support teams; triages customer-impacting issues.
  - Ensures knowledge transfer: playbooks, KB articles, runbooks for common issues.
- Interactions:
  - Alerts Product/PM and Engineering of recurring or critical customer issues.
  - Coordinates post-release support and collects feedback for prioritization.
- When to involve:
  - During release planning, incident triage, and when preparing customer-facing docs.

### Accessibility Advocate
- Responsibilities:
  - Ensures accessibility considerations are embedded in design and QA.
  - Conducts accessibility reviews and coordinates remediation.
- Interactions:
  - Partners with UX Researcher, Developers, and QA to add accessibility acceptance criteria and tests.
- When to involve:
  - At design review and before release for accessibility validation.

---

## How these personas improve outcomes
- Clarifies ownership for cross-cutting concerns (releases, infrastructure, observability, accessibility).
- Speeds decisions by surfacing the right stakeholders early.
- Improves quality and supportability through defined handoffs and accountable roles.
- Makes onboarding easier by providing concrete responsibilities and touchpoints.

---

## Using these personas
- Add people to project role fields in the project README or project board cards.
- For every major work item, explicitly list the persona owners for release, platform, data, UX, and support where applicable.
- Update the risk register and release checklist to include owners from these personas when relevant.
