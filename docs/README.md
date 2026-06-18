# OctoAcme Project Management Docs

## Quick Summary

OctoAcme follows an iterative, customer-first project management approach with clear ownership and a lightweight set of artifacts to enable reliable delivery. Core practices include short feedback loops (sprints/milestones), defined roles (PM, Product Manager, Developers, QA), a shared backlog with acceptance criteria, regular demos and retrospectives, and an explicit risk register and escalation path.

### Project Lifecycle & Workflows

OctoAcme follows a structured five-phase project lifecycle: Initiation, Planning, Execution, Release, and Close & Retrospective. The process begins with creating a lightweight Project One-pager that defines the business need, success metrics, and stakeholder alignment—serving as a decision gate before moving into detailed planning. Once approved, the Planning phase breaks work into a prioritized backlog with clear acceptance criteria, estimates, and a release timeline. During Execution, the team works in sprints or iterations using a GitHub Projects board with standardized columns (Backlog, Ready, In Progress, In Review, QA, Done), supported by daily 15-minute standups, weekly delivery syncs, and end-of-sprint demos. Pull requests are kept small (≤400 lines when possible) and require at least one approval before merging. This iterative, customer-first approach emphasizes delivering testable increments while maintaining clear ownership and data-informed decision-making.

### Roles, Communication & Governance

OctoAcme defines three core delivery personas: **Product Managers** who own the vision, prioritize the backlog, and measure outcomes; **Project Managers** who coordinate schedules, manage risks, and maintain transparency; and **Developers** who implement features, write tests, and identify technical risks. A weekly sync between PM and Product Manager, twice-weekly standups for the delivery team, and monthly stakeholder updates form the communication cadence. Risk management is centralized in a Risk Register (maintained with ID, Description, Impact, Likelihood, Owner, Mitigation, and Status), reviewed weekly. Escalation follows a clear three-level path: team-level triage → PM escalation to Product Lead and dependent teams → sponsor-level escalation for business-impacting issues. This structured communication ensures alignment, reduces surprises, and enables rapid response to blockers.

### Quality Assurance & Continuous Improvement

Quality is built into OctoAcme's execution model through multiple layers: unit tests and integration tests for new logic, end-to-end smoke tests for critical flows before release, security scanning in CI, and manual QA for feature acceptance when needed. All code changes must pass automated tests and linting before review. Before any release, pre-release requirements include verification that all acceptance criteria are met, CI and security scans pass, release notes are drafted, and a rollback plan is documented. After each sprint, release, or milestone, the team conducts a blameless retrospective (45–75 minutes) to capture learnings, identify improvements, and generate 2–3 prioritized action items. These improvements are tracked as backlog items with clear owners and timelines, reviewed in weekly PM syncs, and measured for impact—embedding continuous learning into the culture.

## Docs Index

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## How to Use

- **Start here**: Read the [Project Management Overview](./octoacme-project-management-overview.md) for a high-level view of OctoAcme's approach and core principles.
- **Starting a new project**: Use the [Project Initiation Guide](./octoacme-project-initiation.md) to validate the business need, align stakeholders, and create your Project One-pager.
- **Planning & delivery**: Follow the [Project Planning](./octoacme-project-planning.md) and [Execution & Tracking](./octoacme-execution-and-tracking.md) docs during active delivery and sprint cycles.
- **Managing risk**: Track risks in the Risk Register and surface blockers through the escalation path outlined in [Risk Management & Communication](./octoacme-risks-and-communication.md).
- **Releasing to production**: Use the [Release & Deployment Guide](./octoacme-release-and-deployment.md) to standardize deployments and reduce risk.
- **Learning & improvement**: Run retrospectives after sprints, releases, or milestones using the [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) guide.
- **Understanding roles**: Refer to [Roles & Personas](./octoacme-roles-and-personas.md) for role definitions and responsibilities.

---

**Note:** This README is the canonical index for OctoAcme project management process documents. For updates or additions to process docs, please submit an issue using the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template.
