# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup.
- Level 2: PM escalates to Product Lead and dependent teams; SRE/DevOps engaged for infrastructure or deployment blockers.
- Level 3: Sponsor-level escalation for business-impacting issues; Release Manager notified for any release-blocking incidents.

## Execution Checklist
- [ ] Branching and PR conventions documented in repo.
- [ ] CI configured for tests and lint.
- [ ] Regular demos scheduled.
- [ ] Risk register updated weekly.
- [ ] SRE / DevOps pipeline health verified before each release.
- [ ] Release Manager assigned and release window confirmed.
- [ ] [Release Readiness Checklist](./checklists/release-readiness-checklist.md) completed and all role sign-offs collected before deploying to production.
