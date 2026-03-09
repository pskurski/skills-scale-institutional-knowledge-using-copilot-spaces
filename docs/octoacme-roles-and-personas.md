# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

> **Related resources:**
> - [Role Interaction Matrix](./checklists/role-interaction-matrix.md) — RACI table mapping all personas to lifecycle activities.
> - [Release Readiness Checklist](./checklists/release-readiness-checklist.md) — per-role sign-off checklist for production releases.

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

## UX Designer

### Role Summary
UX Designers advocate for the end user throughout the product lifecycle. They translate user research and product goals into clear, testable designs that development and QA can implement and validate.

### Responsibilities
- Conduct user research, usability testing, and competitive analysis.
- Create wireframes, prototypes, and high-fidelity design specifications.
- Define and maintain design system components and interaction patterns.
- Review implemented features for design fidelity and accessibility compliance.
- Partner with QA on usability acceptance criteria.

### Goals
- Ensure product experiences are intuitive, accessible (WCAG 2.1 AA), and aligned with user needs.
- Reduce costly late-stage design changes by involving design earlier in the cycle.
- Build a shared design language that speeds up delivery.

### Typical Communication
- Design review sessions with PdM and Developers before and during sprints.
- Annotated prototypes and design specs shared in the project repo or design tool.
- Usability test findings presented to PM and PdM.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PdM, BA | Feature scope, user stories, usability acceptance criteria |
| Development | Developers | Design specs, component guidance, implementation review |
| QA | QA | Usability and accessibility test cases |
| Release | PM, Release Manager | UI sign-off in release readiness checklist |

---

## SRE / DevOps

### Role Summary
Site Reliability Engineers and DevOps Engineers own the deployment pipeline, infrastructure reliability, and operational health of OctoAcme services. They bridge development and operations to ensure stable, observable, and recoverable systems.

### Responsibilities
- Design, maintain, and improve CI/CD pipelines and deployment automation.
- Monitor system health, set SLOs/SLAs, and respond to incidents.
- Conduct capacity planning and performance testing.
- Document and validate rollback procedures for every release.
- Partner with Security Lead on infrastructure compliance and hardening.
- Update on-call schedules and incident runbooks.

### Goals
- Maintain agreed service reliability targets (uptime, error rate, latency).
- Reduce mean time to recovery (MTTR) for incidents.
- Automate toil and increase deployment frequency safely.

### Typical Communication
- Incident post-mortems and reliability reviews.
- Deployment and infrastructure change notifications to PM.
- CI/CD pipeline status visible to the full delivery team.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PM, Tech Lead | Infrastructure capacity, deployment constraints |
| Development | Developers, Tech Lead | Pipeline configuration, environment setup |
| QA | QA | Performance and reliability test execution |
| Release | Release Manager, PM | Deployment execution, rollback readiness, monitoring setup |
| Post-Release | Security Lead, PM | Incident response, monitoring, post-mortem |

---

## Business Analyst

### Role Summary
Business Analysts translate business objectives into actionable requirements. They bridge stakeholders and the delivery team to ensure the right problems are being solved in the right way.

### Responsibilities
- Elicit, document, and validate business and functional requirements.
- Create user stories, process flows, and acceptance criteria in collaboration with PdM.
- Analyze workflow gaps and propose process improvements.
- Facilitate requirement workshops with stakeholders.
- Ensure requirements remain traceable through delivery.

### Goals
- Eliminate ambiguity in requirements before development begins.
- Ensure delivered features map clearly to business value.
- Reduce rework caused by misunderstood requirements.

### Typical Communication
- Requirement workshops and stakeholder interviews.
- Documented user stories and process flow diagrams shared with PM and PdM.
- Acceptance criteria walk-throughs with QA and Developers.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Initiation | PdM, Stakeholders | Problem framing, business case |
| Planning | PM, PdM, Developers | User stories, acceptance criteria, process flows |
| Development | Developers, QA | Clarifying requirements, reviewing builds against criteria |
| Release | PM | Confirming scope aligns with original business intent |

---

## Data Scientist / Analyst

### Role Summary
Data Scientists and Analysts support data-informed decision-making across the product lifecycle. They design experiments, analyze product metrics, and help the team understand whether the right outcomes are being achieved.

### Responsibilities
- Define measurement plans and success metrics in collaboration with PdM.
- Instrument features and validate tracking in staging and production.
- Analyze experiment results and product usage data; surface insights.
- Prototype predictive models or data-driven features when needed.
- Maintain dashboards and reports for ongoing monitoring.

### Goals
- Ensure every feature has clear, measurable success criteria.
- Provide fast, reliable insights that drive roadmap decisions.
- Minimize data quality issues that could mislead product decisions.

### Typical Communication
- Measurement plans shared with PdM and PM at planning time.
- Experiment results and metric reports distributed to Stakeholders and PdM.
- Data pipeline and dashboard updates communicated to Developers and SRE.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PdM, BA | Defining success metrics and measurement plan |
| Development | Developers, SRE | Tracking implementation, data pipeline changes |
| QA | QA | Verifying analytics events in staging |
| Release | Release Manager | Confirming analytics instrumentation in release readiness |
| Post-Release | PdM, Stakeholders | Reporting on outcomes, informing next iteration |

---

## Support / Customer Success

### Role Summary
Support and Customer Success team members act as the voice of the customer within the delivery process. They surface real-world pain points, ensure smooth rollouts, and help customers adopt new features.

### Responsibilities
- Share support ticket trends and customer feedback with PdM and PM.
- Participate in release planning to flag potential support impact.
- Create or update support runbooks, FAQs, and help center articles.
- Brief the support team on upcoming changes before release.
- Coordinate escalation paths for customer-impacting incidents.

### Goals
- Reduce post-release support ticket volume through proactive documentation.
- Ensure customers successfully adopt new features.
- Close the feedback loop between customers and the product team.

### Typical Communication
- Regular feedback summaries shared with PdM and PM.
- Release briefings ahead of deployments.
- Post-release customer sentiment and ticket trend reports.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PdM, PM | Flagging customer pain points, informing priority |
| Development | PdM, BA | Reviewing features for customer usability |
| Release | PM, Release Manager | Support readiness sign-off, customer communication plan |
| Post-Release | PM, PdM | Escalating customer-impacting issues, measuring adoption |

---

## Security Lead

### Role Summary
The Security Lead ensures that OctoAcme products and processes meet security and compliance requirements. They embed security practices throughout the lifecycle rather than treating security as a final gate.

### Responsibilities
- Define security requirements and threat models for new features and integrations.
- Review architecture and code for security risks.
- Run and interpret SAST, DAST, and dependency vulnerability scans.
- Coordinate incident response for security events.
- Validate post-release security posture and compliance artifacts.
- Partner with SRE/DevOps on infrastructure hardening and access controls.

### Goals
- Shift security left to catch issues early and cheaply.
- Ensure no critical unmitigated security findings ship to production.
- Build a culture where security is a shared responsibility.

### Typical Communication
- Threat model reviews shared with PM, PdM, and Developers early in planning.
- Security scan reports distributed before release reviews.
- Incident response communication coordinated with PM and SRE.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PdM, BA, Tech Lead | Threat modeling, security requirements |
| Development | Developers, SRE | Secure coding guidance, dependency reviews |
| QA | QA, SRE | Security test execution, scan results review |
| Release | Release Manager, PM | Security sign-off in release readiness checklist |
| Post-Release | SRE, PM | Monitoring for security events, incident response |

---

## Release Manager

### Role Summary
The Release Manager owns the end-to-end release process. They coordinate all stakeholders, enforce the release readiness checklist, and hold the authority to approve or defer releases.

### Responsibilities
- Define and maintain the release process and cadence.
- Coordinate release windows with PM, SRE/DevOps, and Stakeholders.
- Drive the release readiness review and collect sign-offs from all required personas.
- Communicate release status and go/no-go decisions to the team.
- Manage hotfix and rollback processes for failed releases.
- Maintain a release calendar and changelog.

### Goals
- Deliver releases on schedule with minimal disruption.
- Ensure every release meets quality, security, and operational readiness standards.
- Provide clear communication before, during, and after releases.

### Typical Communication
- Release schedule published to PM, PdM, and Stakeholders.
- Go/no-go announcements via team channels.
- Post-release summaries including any incidents or deferred items.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PM, SRE/DevOps | Release calendar, deployment window planning |
| QA | QA, SRE/DevOps | Release gate criteria, readiness review |
| Release | All personas | Collecting sign-offs via release readiness checklist |
| Post-Release | PM, SRE, Support/CS | Confirming release success, managing rollbacks if needed |

---

## Technical Lead

### Role Summary
The Technical Lead provides architectural guidance, sets engineering standards, and acts as the primary technical decision-maker for the delivery team.

### Responsibilities
- Define and maintain the technical architecture and design standards.
- Review technical designs, PRs, and implementation decisions.
- Identify and mitigate technical risks and dependencies.
- Mentor developers and facilitate knowledge sharing.
- Collaborate with SRE/DevOps on infrastructure and deployment architecture.
- Act as the escalation point for complex technical blockers.

### Goals
- Ensure the codebase remains maintainable, scalable, and secure.
- Reduce technical debt while meeting delivery timelines.
- Align technical decisions with product goals and business constraints.

### Typical Communication
- Architecture decision records (ADRs) shared with PM, PdM, and Developers.
- Technical risk items surfaced in the risk register.
- Code and design review participation throughout sprints.

### Interactions
| Phase | Collaborates With | On What |
|-------|------------------|---------|
| Planning | PM, PdM, BA | Feasibility, effort estimates, technical constraints |
| Development | Developers, SRE/DevOps | Architecture, code quality, pipeline design |
| QA | QA, SRE/DevOps | Test strategy for complex technical components |
| Release | Release Manager, SRE/DevOps | Technical readiness, deployment architecture sign-off |
| Post-Release | SRE/DevOps, PM | Post-mortem technical analysis, debt backlog |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For cross-role coordination, consult the [Role Interaction Matrix](./checklists/role-interaction-matrix.md).
- For release gates and sign-offs, use the [Release Readiness Checklist](./checklists/release-readiness-checklist.md).

