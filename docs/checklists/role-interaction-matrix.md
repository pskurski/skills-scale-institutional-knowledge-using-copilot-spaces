# OctoAcme Role Interaction Matrix

This matrix maps key project lifecycle activities to personas using a lightweight RACI format:

| Symbol | Meaning |
|--------|---------|
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — owns the outcome; gives final sign-off |
| **C** | **Consulted** — provides input before/during |
| **I** | **Informed** — kept up to date |

---

## RACI Matrix

| Activity | PM | PdM | Dev | QA | UX | SRE/DevOps | BA | Data Scientist/Analyst | Support/CS | Security | Release Mgr | Tech Lead |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Initiation — Problem Definition** | C | A/R | I | I | C | I | R | C | C | I | I | I |
| **Initiation — Stakeholder Alignment** | R | A | I | I | I | I | C | I | C | I | I | I |
| **Planning — Requirements & Scope** | A | R | C | C | C | C | R | C | C | I | C | C |
| **Planning — Sprint / Iteration Planning** | A | C | R | C | C | C | I | I | I | I | I | R |
| **Planning — Risk Register** | R | C | C | C | I | C | C | I | I | C | I | C |
| **Development — Feature Implementation** | I | C | R | C | C | I | I | I | I | I | I | A |
| **Development — UX / Design Review** | I | C | C | I | A/R | I | I | I | I | I | I | I |
| **Development — Security Review** | I | I | C | I | I | C | I | I | I | A/R | I | C |
| **QA — Acceptance Testing** | I | A | C | R | C | C | C | I | I | I | I | C |
| **QA — Performance / Load Testing** | I | I | C | R | I | A/R | I | I | I | I | I | C |
| **Release — Release Readiness Review** | A | C | C | C | C | C | I | C | C | C | R | C |
| **Release — Deployment** | I | I | C | I | I | R | I | I | I | C | A | C |
| **Release — Go / No-Go Decision** | A | C | C | C | I | C | I | I | I | C | R | C |
| **Post-Release — Monitoring & Incident Response** | I | I | C | I | I | R | I | C | I | C | A | C |
| **Post-Release — Support Handoff** | C | C | I | I | I | I | I | I | A/R | I | I | I |
| **Post-Release — Metrics & Analysis** | I | A | I | I | I | I | I | R | C | I | I | I |
| **Retrospective — Facilitation** | R | C | C | C | C | C | C | C | C | C | C | C |
| **Retrospective — Action Items** | A | C | R | R | R | R | R | R | R | R | R | R |

---

## Notes on Key Interactions

### Initiation
- **PM** and **PdM** set scope; **BA** documents business requirements; **Data Analyst** provides market/usage baseline.

### Planning
- **BA** translates business needs to user stories; **Tech Lead** reviews feasibility; **SRE/DevOps** flags infrastructure constraints.

### Development
- **Tech Lead** guides architectural decisions; **UX Designer** provides design specs; **Security Lead** conducts threat modeling early.

### QA
- **QA** owns test execution; **SRE/DevOps** owns performance/reliability tests; **UX Designer** validates UX acceptance.

### Release
- **Release Manager** coordinates the release window; **SRE/DevOps** executes deployment; **PM** owns go/no-go; see [Release Readiness Checklist](./release-readiness-checklist.md).

### Post-Release
- **SRE/DevOps** monitors and leads incident response; **Support/CS** manages customer impact; **Data Analyst** validates success metrics.

---

*See also: [Release Readiness Checklist](./release-readiness-checklist.md) | [Roles & Personas](../octoacme-roles-and-personas.md)*
