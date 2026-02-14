# Risk Matrix (Risk-Based Testing)

## Scale
- Probability: 1 (Low) to 5 (High)
- Impact: 1 (Low) to 5 (High)
- Risk Score = Probability x Impact

## Risk Table

| Risk | Probability | Impact | Score | Mitigation | Test Focus |
|------|-------------|--------|-------|------------|------------|
| Payment/transaction failure | 3 | 5 | 15 | Contract/API validations + E2E smoke on payments | API + E2E |
| Authentication instability | 4 | 4 | 16 | Smoke tests + negative cases + rate limit checks | API + UI |
| Data inconsistency between services | 3 | 4 | 12 | Integration tests + reconciliation checks | Integration |
| High flakiness on UI tests | 4 | 3 | 12 | Stabilize selectors, retries policy, reduce E2E scope | Automation stability |
| Regression in core journey | 3 | 5 | 15 | Core regression suite + risk-based selection | Regression |

## Prioritization
- 15–25: Must test before release (blocker if not covered)
- 8–14: Should test (release with mitigation)
- 1–7: Nice to have (monitor)
