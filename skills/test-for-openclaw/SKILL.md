---
name: test-for-openclaw
description: Require evidence before declaring coding work done in OpenClaw. Use when the request sounds like "verify this works", "what tests should we add", "prove this is safe", "is this ready", or any implementation, fix, refactor, review, or deploy task where the right level of proof is ambiguous or easy to under-scope.
---

# Test For OpenClaw

Completion requires proof.

## Process

1. Identify the real behavior at risk.
2. Choose the cheapest credible form of evidence.
3. Run verification as close as possible to the changed surface.
4. Record what passed, what was not run, and why.
5. Refuse to overclaim when evidence is partial.

## Acceptable Evidence

- targeted automated tests
- lint or typecheck on affected code
- browser-based flow verification for UI changes
- reproduction before and after for bug fixes
- diff inspection for prompt or documentation-only work

## Reference Files

Read `references/evidence-ladder.md` when you need to choose the minimum credible proof for a change.

## Bad Evidence

- confidence without execution
- "looks right"
- passing unrelated tests
- assumptions about triviality
