# Test Plan (Release / Sprint)

## 1. Release Overview
- Release name: Example Release v1.0
- Sprint: Sprint 12
- Target date: YYYY-MM-DD
- Main changes: New feature X, API changes, bug fixes

## 2. Test Scope
- Feature X end-to-end flow
- API endpoints: /auth, /orders, /payments (example)
- Regression: login, onboarding, checkout, profile

## 3. Test Execution Plan
### Phase 1 — Smoke (CI Gate)
- Runs on each deploy
- Focus: app up + core endpoints responding

### Phase 2 — Functional Validation
- Validate acceptance criteria
- Cover main happy paths + essential negative cases

### Phase 3 — Regression
- Run core journey suite
- Validate no regression in high-risk areas

### Phase 4 — Exploratory
- Timeboxed session on risk areas
- Focus on edge cases and integration behavior

## 4. Roles & Responsibilities
- QA: plan, execute, report, coordinate quality gates
- Dev: fix, support debugging, provide logs
- PO/BA: confirm business rules, prioritize risks

## 5. Test Evidence
- Automation reports
- API collections results
- Screenshots/videos for failed UI tests
- Test report summary

## 6. Risks & Mitigations
Reference: docs/03-risk-matrix.md
