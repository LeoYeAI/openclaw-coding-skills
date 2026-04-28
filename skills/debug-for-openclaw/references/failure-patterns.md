# Failure Patterns

## Intermittent Failure

Likely signals:

- timing sensitivity
- hidden state coupling
- environment dependence
- test pollution or missing isolation

## After A Refactor

Likely signals:

- preserved behavior was assumed rather than proved
- boundary contracts shifted subtly
- old call paths were not fully replaced

## After Config Or Environment Change

Likely signals:

- missing defaults
- stale assumptions about runtime wiring
- wrong startup order
- hidden dependency on environment variables or external services

## Rule

Use the failure pattern as a hypothesis generator, not as proof.
