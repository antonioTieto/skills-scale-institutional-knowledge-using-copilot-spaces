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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas

To reduce ambiguity on cross-cutting responsibilities and speed up decision making, add the following personas to the project process docs. Each entry includes Responsibilities and Interaction notes describing handoffs with existing roles.

- Release Manager
  - Responsibilities:
    - Coordinate release windows across teams and regions
    - Maintain and own the release checklist and rollback plan
    - Validate production readiness and sign off on releases
    - Liaise with on-call, Support, and Communications for rollouts
  - Interaction:
    - Works with PM to schedule releases and communicate stakeholder timelines
    - Coordinates with DevOps/Platform Engineer on pipeline gating and deployment steps
    - Notifies Stakeholder Representative and Support for release announcements and post-release monitoring

- Tech Lead
  - Responsibilities:
    - Provide technical direction and architectural leadership
    - Approve significant architecture decisions and trade-offs
    - Mentor developers and help unblock technical progress
    - Own non-functional requirements (performance, scalability)
  - Interaction:
    - Partners with PdM/PM to discuss technical trade-offs and delivery estimates
    - Works with Developers to ensure implementation meets architecture and DoD

- UX Researcher / Designer
  - Responsibilities:
    - Lead user research and usability validation
    - Produce design artifacts and acceptance criteria for user-facing flows
    - Validate designs during implementation and testing
  - Interaction:
    - Collaborates with PdM to define user outcomes and acceptance criteria
    - Works with Developers and QA to ensure designs are implementable and tested

- Data Analyst / Analytics Owner
  - Responsibilities:
    - Define and document success metrics and instrumentation needs
    - Validate data quality and author metric queries/dashboards
    - Monitor metrics post-release for expected impact
  - Interaction:
    - Partners with PdM to set measurable outcomes and targets
    - Receives instrumentation PRs from Developers and verifies telemetry
    - Shares dashboards with PM and stakeholders for decision-making

- DevOps / Platform Engineer
  - Responsibilities:
    - Maintain CI/CD pipelines and deployment automation
    - Own infrastructure-as-code and production reliability patterns
    - Define deployment patterns and support incident recovery
  - Interaction:
    - Supports Developers and Release Manager for safe deployments
    - Works with PM on operational capacity considerations and environment readiness

- Compliance / Security Owner
  - Responsibilities:
    - Capture regulatory and security requirements for features
    - Run security reviews and sign off on compliance checklists
    - Coordinate remediation plans with engineering
  - Interaction:
    - Engages with PdM and Tech Lead during planning for required controls
    - Works with Release Manager to ensure compliance steps are completed before release

- Stakeholder Representative (Business SME)
  - Responsibilities:
    - Represent business priorities and domain knowledge
    - Validate acceptance criteria and approve stakeholder-facing decisions
    - Provide context for trade-offs impacting business outcomes
  - Interaction:
    - Works with PdM and PM to clarify scope and sign off on release communications
    - Supports acceptance and validation with end-user perspectives

Example handoffs (short)
- Release checklist handoff: Tech Lead / DevOps confirm CI/CD and infra readiness -> Release Manager validates rollback and post-release plan -> PM schedules communication with Stakeholder Representative and Support.
- Instrumentation handoff: Data Analyst defines metrics and events -> Developer implements instrumentation PR with required fields -> Data Analyst validates and publishes dashboards.
