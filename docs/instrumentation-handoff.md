# Instrumentation & Analytics Handoff Template

Purpose: Standard template to ensure product changes have measurable telemetry and clear analytics ownership.

Pre-implementation
- Owner: Data Analyst / Analytics Owner
- [ ] Define success metrics (primary and secondary)
- [ ] Specify events and fields required, including data types and privacy considerations
- [ ] Provide example dashboard or queries to validate metrics

Implementation
- [ ] Developer implements events with the required schema and tests
- [ ] Include documentation in PR describing events and expected property values
- [ ] Add automated tests or validations for telemetry where possible

Validation & Release
- [ ] Data Analyst validates data quality in staging and production
- [ ] Dashboard queries return expected values for test scenarios
- [ ] Data Analyst signs off before release (or flags gaps to Release Manager/Tech Lead)

Post-release
- [ ] Monitor metrics for expected behavior during the monitoring window
- [ ] Log discrepancies and assign remediation tasks if needed

Example event spec:
- event_name: "checkout_completed"
- properties:
  - user_id: string (hashed)
  - total_value: number
  - currency: string
  - promo_code: string (nullable)

Notes:
- Ownership: Data Analyst ensures metrics are defined and validated; Developers implement instrumentation.
- Interaction: Instrumentation is a shared responsibility — implementers must follow the Analytics Owner's spec.
