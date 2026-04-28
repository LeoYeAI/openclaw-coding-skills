# Rollback Patterns

## When To Plan Rollback Explicitly

Do not treat rollback as optional when:

- config changes can disable critical paths
- migrations can leave data or state in a mixed condition
- external service wiring is changing
- startup behavior or environment assumptions are shifting

## Rollback Questions

- What exact state change would need to be undone?
- Can rollback be immediate, or does it require operator steps?
- What happens if rollback succeeds only partially?
- Is there a safe fallback mode if full rollback is impossible?

## Practical Rule

If the change affects production behavior and you cannot explain the rollback path in a few sentences, release confidence is overstated.
