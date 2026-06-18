# Release Manager Checklist (Template)

Purpose: Standard checklist to use for production releases to ensure readiness and reduce risk.

Pre-release (before scheduled window)
- [ ] Confirm target commit/PRs for release and document release notes
- [ ] Verify all acceptance criteria for included PRs are met
- [ ] Ensure CI is green and security scans have passed
- [ ] Confirm rollback plan and that previous-good build is available
- [ ] Validate monitoring/dashboards and alerting are in place for key metrics
- [ ] Notify Support, Communications, and Stakeholder Representative of planned release

Deployment
- [ ] Run deployment to staging and execute smoke tests
- [ ] Run canary/gradual rollout (if applicable) and monitor metrics
- [ ] Verify health checks and key transactions manually or via smoke tests
- [ ] If any blocking issue is detected, execute rollback plan

Post-release
- [ ] Confirm post-deploy verifications and close monitoring window
- [ ] Announce release completion to stakeholders and Support
- [ ] Log any issues and create follow-up action items in the project board
- [ ] Update release notes with any post-release findings

Notes:
- Ownership: Release Manager owns checklist execution and sign-off.
- Interactions: Coordinate with DevOps for pipeline steps and Tech Lead for technical sign-off.
