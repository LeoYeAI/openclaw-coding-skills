# Review Finding Template

Use this structure for findings.

## Format

- severity: high | medium | low
- area: correctness | regression | security | verification | maintainability
- claim: what is wrong
- evidence: what in the change suggests the issue
- consequence: why it matters
- fix direction: what to change or verify

## Example Skeleton

- severity: medium
- area: verification
- claim: the new branch is unproven under failure conditions
- evidence: tests cover the success path only
- consequence: the change may regress silently on invalid input
- fix direction: add one failing-input test or reproduce the behavior manually
