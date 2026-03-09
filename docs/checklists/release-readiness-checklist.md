# OctoAcme Release Readiness Checklist

Use this checklist before every production release to confirm all roles have completed their pre-release responsibilities. Each item must be checked off by the responsible persona before the Release Manager grants final approval.

---

## 1. Product & Scope (Product Manager — PdM)
- [ ] Acceptance criteria for all release items are met and documented.
- [ ] Feature flags and rollout scope are confirmed.
- [ ] Release notes draft reviewed and approved.
- [ ] Any scope changes since last planning cycle are communicated to PM.

**Sign-off:** PdM confirms release scope is complete and ready. ✅

---

## 2. Schedule & Dependencies (Project Manager — PM)
- [ ] Release date and deployment window are scheduled and communicated.
- [ ] All cross-team dependencies are resolved or risk-accepted.
- [ ] Stakeholder notification sent (at least 24 hours before release).
- [ ] Go / no-go decision documented in the risk register.

**Sign-off:** PM confirms logistics are in order. ✅

---

## 3. Engineering & Quality (Developers + QA)
- [ ] All code merged to release branch; no open blocking PRs.
- [ ] CI pipeline green (tests, lint, build).
- [ ] Unit, integration, and end-to-end smoke tests pass.
- [ ] Manual QA completed for critical user flows.
- [ ] No P0/P1 defects open against release scope.

**Sign-off:** Engineering Lead and QA Lead confirm quality bar met. ✅

---

## 4. Infrastructure & Reliability (SRE / DevOps)
- [ ] Deployment pipeline tested against staging environment.
- [ ] Rollback procedure documented and validated.
- [ ] Monitoring dashboards and alerts configured for the new release.
- [ ] Load/performance baseline checked; capacity confirmed.
- [ ] On-call schedule updated for release window.

**Sign-off:** SRE / DevOps confirms infrastructure is release-ready. ✅

---

## 5. Security (Security Lead)
- [ ] Security scan (SAST/DAST/dependency scan) run with no unmitigated critical findings.
- [ ] Threat model reviewed for new features or data flows.
- [ ] Secrets and credentials rotated or verified as not exposed.
- [ ] Compliance requirements satisfied (e.g., data privacy, access controls).

**Sign-off:** Security Lead confirms no outstanding security blockers. ✅

---

## 6. Design & Usability (UX Designer)
- [ ] Final UI matches approved designs; no critical UX regressions.
- [ ] Accessibility requirements met (WCAG 2.1 AA minimum).
- [ ] User-facing copy reviewed and approved.

**Sign-off:** UX Designer confirms design fidelity and accessibility. ✅

---

## 7. Data & Analytics (Data Scientist / Analyst)
- [ ] Tracking events verified in staging; data pipelines updated.
- [ ] Success metrics and measurement plan documented.
- [ ] Dashboards updated to reflect new features or changes.

**Sign-off:** Data Analyst confirms instrumentation is correct. ✅

---

## 8. Support Readiness (Support / Customer Success)
- [ ] Support runbook / FAQ updated with new feature info.
- [ ] Customer-facing release notes or changelog prepared.
- [ ] Support team briefed on expected changes and common questions.

**Sign-off:** Support / Customer Success Lead confirms team readiness. ✅

---

## 9. Final Release Approval (Release Manager)
- [ ] All section sign-offs above are completed.
- [ ] Release ticket / PR updated with checklist link.
- [ ] Post-release monitoring window defined (minimum 30 minutes of active watch post-deployment).
- [ ] Incident response contacts confirmed for release window.

**Sign-off:** Release Manager approves release to proceed. ✅

---

## Success Criteria
The release is considered successful when:
- All production monitors remain green for a minimum of 30 minutes post-deployment.
- Error rate does not exceed agreed threshold (e.g., < 0.1% increase).
- No P0/P1 incidents opened within the first hour.
- Rollback is not triggered.

---

*See also: [Role Interaction Matrix](./role-interaction-matrix.md) | [Roles & Personas](../octoacme-roles-and-personas.md)*
