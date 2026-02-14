# Test Strategy

## 1. Objective
Ensure reliable releases by embedding quality throughout the SDLC, reducing production risks through risk-based testing, automation, and clear quality gates.

## 2. Scope
### In scope
- Web UI critical flows
- REST APIs (contract and business validation)
- Integrations between services
- Regression suite for core business journeys

### Out of scope (example)
- 3rd-party provider internal validations (only contract tests)
- Non-critical UI cosmetic checks (unless affects usability)

## 3. Quality Goals
- Prevent critical defects in production
- Maintain stable CI/CD feedback loops
- Provide confidence for deployments through measurable signals

## 4. Test Levels & Types
- Smoke tests (fast, deploy gate)
- Functional tests (UI + API)
- Regression tests (core journeys)
- Contract tests (API schema/contract)
- Exploratory testing (risk areas / new features)
- Non-functional (baseline performance checks when applicable)

## 5. Approach (Risk-Based Testing)
We prioritize tests based on:
- Business criticality (financial impact / compliance / churn)
- Frequency of use (high traffic flows)
- Complexity (many integrations, complex rules)
- Change rate (modules with frequent releases)
- History (areas with recurring incidents)

## 6. Automation Strategy
### What to automate
- Stable and high-value regressions
- Smoke tests for CI gates
- API validations for business rules and critical responses

### What to keep manual
- Early-stage features
- UX exploratory sessions
- One-off scenarios where automation cost outweighs benefit

## 7. Environments & Data
- Use isolated test data when possible
- Prefer data factories / seeded datasets for automation
- Ensure environment health checks before execution

## 8. Tooling (example)
- UI: Cypress / Selenium
- API: Postman / SoapUI
- CI/CD: GitHub Actions / GitLab CI (example)
- Reporting: Allure / HTML reports (optional)

## 9. Metrics (Signals)
- Defect leakage (prod vs. pre-prod)
- Automation pass rate & flakiness rate
- Escape rate by severity
- Mean time to detect (MTTD) and mean time to fix (MTTF)
- Test coverage by risk category

## 10. Definition of Done (Quality)
- Acceptance criteria validated
- Smoke suite green
- No open critical defects
- Regression executed for impacted areas
- Test evidence attached (logs, screenshots, report links)

## Engineering Mindset

Quality Engineering is not tool-driven — it is impact-driven.

Tools may change (Cypress, Playwright, Selenium), but principles remain:

- Protect business-critical flows first
- Automate what adds confidence
- Use metrics, not intuition
- Communicate risks clearly
- Own release decisions alongside engineering

A senior QA does not execute tasks.
A senior QA protects the product.

