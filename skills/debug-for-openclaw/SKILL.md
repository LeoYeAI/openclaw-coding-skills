---
name: debug-for-openclaw
description: Triage and resolve failures inside an OpenClaw workspace with a disciplined debugging loop. Use when the request sounds like "help me debug this", "this test is failing", "the build broke", "this works sometimes and I do not know why", or when logs suggest a problem but not the cause.
---

# Debug For OpenClaw

Debug by narrowing uncertainty, not by guessing fixes.

## Process

1. Reproduce the problem as concretely as possible.
2. Define the observed behavior and the expected behavior.
3. Localize the failure surface before editing code.
4. Reduce the problem to the smallest reproducible case you can get.
5. Form one strong hypothesis at a time.
6. Change the narrowest possible surface.
7. Re-run the proof.
8. Add a guard so the same class of failure is less likely to return.

## OpenClaw Guidance

- Prefer first-class tools for inspection when available.
- Use browser-based inspection for UI/runtime bugs when the issue is visible in the browser.
- Use logs and traces as evidence, not as a substitute for reproduction.
- If the bug spans many files, re-enter the planning loop before patching blindly.

## Reference Files

Read `references/triage-loop.md` when debugging is getting noisy or speculative.

Read `references/failure-patterns.md` when the failure is intermittent, followed a refactor, or appeared after config or environment changes.

Read `references/localization-strategies.md` when the bug surface is still too broad and you need to shrink the search space.

## Bad Patterns

- changing code before reproducing the bug
- stacking multiple speculative fixes
- using a passing unrelated test as proof
- stopping at symptom removal without understanding cause
