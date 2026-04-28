# Skill Index

## Workflow Layer

- `openclaw-dev-workflow`: default end-to-end orchestration layer for coding work
- `spec-for-openclaw`: define scope and acceptance criteria before coding
- `plan-for-openclaw`: break work into slices and maintain `plan.md`
- `build-for-openclaw`: implement in narrow, testable increments
- `test-for-openclaw`: require evidence before completion
- `review-for-openclaw`: inspect for bugs, regressions, and verification gaps
- `ship-for-openclaw`: close out with clean diff discipline and release readiness

## Specialist Layer

- `debug-for-openclaw`: localize and resolve failures without speculative edits
- `security-for-openclaw`: reason about trust boundaries, secrets, and permissions
- `frontend-for-openclaw`: deliver user-facing changes with runtime verification
- `docs-for-openclaw`: keep durable project knowledge accurate and useful
- `deploy-for-openclaw`: prepare and execute deployments with rollback awareness
- `refactor-for-openclaw`: simplify code while preserving behavior

## Recommended Default Stack

Start with:

1. `openclaw-dev-workflow`
2. `plan-for-openclaw`
3. `build-for-openclaw`
4. `test-for-openclaw`
5. `review-for-openclaw`
6. `ship-for-openclaw`

Add specialist skills based on codebase risk and task mix.
