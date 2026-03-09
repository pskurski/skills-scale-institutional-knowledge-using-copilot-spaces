# OctoAcme Project Management Docs

OctoAcme runs projects with a lightweight, outcome-driven lifecycle: Initiation (one-pager and stakeholder alignment), Planning (kickoff, prioritized backlog, estimates, Definition of Done), Execution (sprints, PRs, CI, reviews), and Release/Close (deployment checklist, release notes, retrospective). The docs emphasize producing a Project One-pager, a prioritized backlog with clear acceptance criteria, and a simple risk register early so that decisions and trade‑offs are visible and traceable as work moves from Backlog → Ready → In Progress → In Review → QA → Done on the project board.

Workflows are pragmatic and developer-friendly: small, focused pull requests (target <= 400 lines), PRs that link to issues and acceptance criteria, automated CI/linting/security scans before requesting reviews, and at least one approval required to merge. Planning uses t-shirt sizing or story points, timeboxed sprint planning, and a backlog-item template to ensure each work item has owner, estimate, and clear acceptance criteria. Risk and dependency management is formalized—each risk has an owner, impact/likelihood, mitigation, and is reviewed during weekly syncs.

Roles and responsibilities are explicit so ownership is clear: the Project Manager coordinates schedules, risks, and communications; the Product Manager defines success metrics and prioritizes the backlog; developers implement and test; QA validates acceptance criteria; stakeholders provide inputs and approvals. Communication cadence combines daily standups for immediate coordination and blocker triage, a weekly delivery sync and PM/PdM check‑ins for alignment, regular demos at the end of sprints or milestones, and monthly stakeholder updates to keep the broader organization informed.

Quality assurance and release controls are baked into the flow: unit and integration tests for logic, end‑to‑end smoke tests for critical flows, manual QA for feature acceptance when needed, and security scans in CI. Releases follow a checklisted process (staging smoke tests, automated deploy pipeline where possible, post‑deploy verification, and announced release notes) with a clear rollback/incident playbook and escalation paths from team → PM → Product Lead → Sponsor for business‑impacting issues. Retrospectives convert learnings into prioritized action items tied back into the backlog to drive continuous improvement.

Documentation Links:
- docs/octoacme-project-management-overview.md
- docs/octoacme-project-initiation.md
- docs/octoacme-project-planning.md
- docs/octoacme-execution-and-tracking.md
- docs/octoacme-risks-and-communication.md
- docs/octoacme-release-and-deployment.md
- docs/octoacme-retrospective-and-continuous-improvement.md
- docs/octoacme-roles-and-personas.md
