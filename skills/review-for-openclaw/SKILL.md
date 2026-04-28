---
name: review-for-openclaw
description: Critically review a code or prompt change in an OpenClaw workspace before merge or handoff. Use when the request sounds like "review this", "audit this PR", "look for bugs", "sanity-check this implementation", or "tell me what is risky here", especially when regressions, weak assumptions, missing tests, or release risk are concerns.
---

# Review For OpenClaw

Review for failure modes first, not presentation quality.

## Process

1. Identify the claimed intent of the change.
2. Compare the implementation against that intent.
3. Look for bugs, regressions, risk, and missing coverage.
4. Check whether verification is sufficient for the risk level.
5. Report findings ordered by severity.

## Review Priorities

- behavioral correctness
- edge cases and regressions
- verification gaps
- interface consistency
- maintainability risk

## Output Standard

Lead with findings. If there are no findings, say so explicitly and note residual uncertainty.

## Reference Files

Read `references/finding-template.md` when you need a stronger structure for review findings.
