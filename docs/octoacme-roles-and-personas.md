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

# Additional Personas — Recommended Additions

The following operational and cross-functional personas are recommended to reduce ambiguity, clarify handoffs, and ensure accountability across delivery, quality, security, and customer-facing activities.

## Technical Lead

### Role summary
Owns the technical direction for the project and ensures the architecture and engineering approach meet non-functional requirements.

### Responsibilities
- Make architecture and design decisions for the project
- Mentor and coach developers on design and implementation
- Review significant PRs and design proposals
- Identify technical risks and propose mitigations
- Ensure scalability, reliability, and performance considerations are included in planning

### Typical communication
- Weekly or bi-weekly syncs with the delivery team and PM
- Technical design reviews and RFCs
- Ad-hoc design sessions during planning and grooming

### Key handoffs
- Provides design artifacts to Developers and QA
- Communicates technical constraints and estimates to the PM and PdM

### Example acceptance signals
- Architecture design documented and reviewed
- Non-functional requirements captured in acceptance criteria
- No critical performance/security regressions in release smoke tests

### Escalation guidance
Escalate to Project Manager for schedule impacts; escalate to Sponsor for major architectural changes affecting scope or budget.

## Delivery Manager

### Role summary
Focuses on optimizing flow of work across teams, removing process impediments, and coordinating cross-team delivery and calendars.

### Responsibilities
- Track and optimize workflow and SLAs across teams
- Remove process-level impediments and blockers
- Coordinate release schedules, cross-team dependencies, and cutover activities
- Maintain and refine delivery metrics (e.g., cycle time, WIP)

### Typical communication
- Weekly delivery syncs with PMs and Release Engineers
- Escalation briefings for cross-team blockers

### Key handoffs
- Coordinates handoffs between teams for integrations
- Provides release readiness signals to the PM and Release Engineer

### Example acceptance signals
- Reduced cross-team wait times and blocked work
- Clear release windows with all dependencies accounted for

### Escalation guidance
Escalate unresolved cross-team blockers to PM; involve Product Lead if scope adjustments are required.

## UX Researcher / Designer

### Role summary
Validates user needs and delivers UX artifacts that ensure usability and alignment to outcomes.

### Responsibilities
- Run user research and usability testing
- Produce UX specs, prototypes, and acceptance criteria related to usability
- Collaborate with PdM to define user-facing success metrics

### Typical communication
- Design reviews and critique sessions during planning
- Demo and handoff meetings with Developers and QA

### Key handoffs
- Deliver design specs and prototypes to Developers
- Provide acceptance criteria to QA and PM

### Example acceptance signals
- Usability test results meet target success thresholds
- Designs have accessible markup and documented interactions

### Escalation guidance
Escalate unresolved design vs. technical feasibility trade-offs to PdM and Technical Lead.

## Security Lead

### Role summary
Defines security requirements and leads threat modeling and remediation for the project.

### Responsibilities
- Run threat modeling and security reviews for new features
- Define security acceptance criteria and compliance requirements
- Coordinate vulnerability scanning and remediation efforts

### Typical communication
- Security review sessions during design & planning
- Regular updates to PM on security findings that affect schedule

### Key handoffs
- Provides security test requirements to QA and CI owners
- Communicates critical vulnerabilities and remediation plans to PM and on-call teams

### Example acceptance signals
- Threat model completed and reviewed
- No critical vulnerabilities present in production-release scans

### Escalation guidance
Escalate critical security findings immediately to PM and Security Incident Response; notify Sponsor for high business-impact vulnerabilities.

## Release Engineer

### Role summary
Owns build, CI/CD pipelines, and the release/rollback processes to ensure repeatable, low-risk deployments.

### Responsibilities
- Maintain and improve CI/CD pipelines and deployment automation
- Define and document release and rollback procedures
- Validate deployment prerequisites and run post-deploy verification

### Typical communication
- Release planning meetings with Delivery Manager and PM
- Runbooks and deployment notes for stakeholders

### Key handoffs
- Signals release readiness to PM and Support Lead
- Handover to Support on post-release monitoring responsibilities

### Example acceptance signals
- Successful staging-to-prod pipeline runs with automated checks
- Rollback steps tested and verified

### Escalation guidance
Escalate deployment failures to on-call and PM; if systemic, escalate to Sponsor.

## Support Lead / Customer Success Liaison

### Role summary
Represents customer-facing concerns, triages production issues, and channels feedback back to the product and engineering teams.

### Responsibilities
- Triage and prioritize production incidents and customer reports
- Maintain communication with customers and internal stakeholders during incidents
- Collect and synthesize user feedback for PdM and Product teams

### Typical communication
- Incident updates and post-incident summaries
- Regular handoffs to PM/PdM on customer-impacting trends

### Key handoffs
- Escalates high-severity incidents to PM and on-call engineers
- Provides prioritized customer feedback to PdM

### Example acceptance signals
- Timely incident triage and customer communication
- Clear, actionable customer feedback feeding the backlog

### Escalation guidance
Escalate outages and major incidents to PM, PdM, and on-call engineering; involve Sponsor if customer SLAs are at risk.

## Data Analyst

### Role summary
Defines success metrics, ensures proper instrumentation, and provides analysis to inform decisions.

### Responsibilities
- Define and validate metrics and dashboards
- Analyze feature impact and provide post-release insights
- Advise on instrumentation and data collection needs

### Typical communication
- Regular metric reports to PdM and PM
- Analysis reviews during retrospectives and planning

### Key handoffs
- Provides dashboards and metrics to the team prior to launch
- Handoff analysis to PdM for decision-making

### Example acceptance signals
- Key success metrics available and validated
- Analysis informs go/no-go decisions

### Escalation guidance
Escalate data quality or instrumentation blockers to PM and engineering leads.

## Solutions / Systems Architect

### Role summary
Ensures the solution design aligns with platform standards and cross-team integration needs.

### Responsibilities
- Define integration contracts and cross-team interfaces
- Identify systemic risks and recommend mitigations
- Ensure alignment with platform/ops constraints

### Typical communication
- Architecture review boards and design critiques
- Coordination with other architects across teams

### Key handoffs
- Provides integration guidance and constraints to Technical Leads
- Coordinates cross-team interface testing plans

### Example acceptance signals
- Integration contracts documented and agreed
- No unexpected production integration failures

### Escalation guidance
Escalate systemic design risks to PM and Sponsor when they affect schedule or scope.

---

## How to use these persona entries
- Add the relevant persona section to project READMEs or the Project One-pager when onboarding a team.
- Use the acceptance signals as inputs when defining "Definition of Done" for related backlog items.
- Follow escalation guidance when unresolved issues impact delivery or business outcomes.
