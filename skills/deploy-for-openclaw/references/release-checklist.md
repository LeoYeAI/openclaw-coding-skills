# Release Checklist

## Before Release

- confirm requested outcome and release scope
- confirm environment assumptions
- confirm verification results are current
- identify migrations, flags, config changes, or manual steps
- define rollback or mitigation path

## During Release

- execute only the planned steps
- watch for startup, migration, or dependency failures
- avoid mixing unrelated changes into the rollout

## After Release

- verify the critical user path
- check monitoring or logs if available
- record any follow-up work or residual risk
