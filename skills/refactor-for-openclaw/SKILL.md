---
name: refactor-for-openclaw
description: Simplify or restructure code in an OpenClaw workspace while preserving behavior. Use when the request sounds like "clean this code up", "simplify this without changing behavior", "reduce duplication here", "this module is getting hard to maintain", or when readability, structure, or verification quality need improvement without changing intended outcomes.
---

# Refactor For OpenClaw

Refactor to reduce complexity, not to satisfy aesthetic preference.

## Process

1. Define what behavior must remain unchanged.
2. Identify the specific complexity being reduced.
3. Prefer small structural improvements over broad rewrites.
4. Keep public interfaces stable unless the task explicitly includes interface change.
5. Verify that behavior is preserved after each meaningful step.
6. Stop when the code is materially clearer, not merely different.

## Refactor Rules

- Do not mix speculative optimization into a clarity refactor.
- Do not rename or move code without a readability payoff.
- Preserve existing conventions unless the convention itself is the problem.
- Keep the diff explainable to a skeptical reviewer.

## Reference Files

Read `references/refactor-decision-test.md` before broad cleanup or structural edits.

Read `references/scope-guardrails.md` when the refactor is expanding beyond one local concern.

Read `references/behavior-preservation-checks.md` when the code is fragile or the preserved behavior is easy to over-assume.

## OpenClaw Guidance

- Pair this skill with `test-for-openclaw` for behavior-preservation proof.
- If the refactor broadens beyond the original scope, return to planning.
- If the real problem is a bug, debug first and refactor second.
