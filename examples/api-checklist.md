# API Testing Checklist (Senior-Level)

## Contract Validation
- Validate response schema (fields, types, required attributes)
- Validate HTTP status codes for all scenarios
- Validate error contract consistency
- Validate backward compatibility

## Business Rule Validation
- Validate positive and negative scenarios
- Boundary value validation
- Data integrity validation
- Idempotency behavior when applicable

## Security & Access
- Authentication validation (token expiration, invalid token)
- Authorization validation (role-based access)
- Rate limiting behavior
- Input sanitization

## Performance Baseline
- Response time within acceptable SLA
- No significant degradation under normal load
- Validate retry mechanisms

## Integration Behavior
- Validate upstream/downstream system response
- Validate data persistence consistency
- Validate asynchronous flows (if applicable)

## Logging & Observability
- Proper error logs generated
- Trace IDs present (if applicable)
- Monitoring alerts triggered when needed
