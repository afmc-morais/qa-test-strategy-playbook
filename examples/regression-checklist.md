# Regression Testing Checklist (Risk-Based)

## Core Business Flows
- Authentication / Login
- Account creation / onboarding
- Payment / transaction processing
- Critical API endpoints
- Profile updates / data changes

## Integration Points
- External service communication
- Database consistency
- Event-driven flows
- Message queues (if applicable)

## UI Stability
- Core journey navigation
- Forms validation
- Responsive behavior (critical views)

## Automation Stability
- No flakiness in core suites
- Stable selectors
- Retry strategy verified

## Risk Revalidation
- Areas affected by recent changes
- High historical defect areas
- Modules with complex logic

## Release Readiness Check
- No open Critical defects
- High severity defects reviewed
- Known risks documented and communicated
- Regression evidence attached
