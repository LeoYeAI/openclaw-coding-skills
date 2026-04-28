---
name: build-for-openclaw
description: Execute implementation work in small, reviewable slices inside OpenClaw. Use when the request is to "implement this", "make the code change", "add this behavior", "wire this up", or "patch this without rewriting everything", especially when the change should stay narrow and be verified immediately.
---

# Build For OpenClaw

Implement in slices, not in bursts.

## Process

1. Select the smallest meaningful slice from the plan.
2. Read only the files needed for that slice.
3. Reuse local patterns before introducing new abstractions.
4. Edit the narrowest possible surface.
5. Verify immediately after the slice.
6. Update progress before starting the next slice.

## Implementation Rules

- Prefer precise edits over broad rewrites.
- Preserve existing design systems and conventions unless the task explicitly changes them.
- If the change becomes wider than expected, stop and re-plan.
- If there is a specialist skill for the domain, combine it with this one.

## Reference Files

Read `references/slice-patterns.md` when the right slice boundary is unclear or when work is expanding unexpectedly.

## Anti-Rationalization

| Rationalization | Response |
|---|---|
| "I will clean it all up in one pass." | Large passes hide regressions. Keep the diff narrow. |
| "I already know the pattern." | Verify the local pattern before copying it in spirit. |
| "Testing can wait until the end." | Verify per slice to catch breakage early. |
