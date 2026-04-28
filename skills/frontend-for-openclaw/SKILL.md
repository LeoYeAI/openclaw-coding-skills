---
name: frontend-for-openclaw
description: Build or modify user-facing interfaces inside an OpenClaw workspace with strong interaction, responsiveness, and verification discipline. Use when the request sounds like "build this UI", "fix this page", "this interaction is broken", "make this responsive", "update this component", or any browser-facing change users will directly see, click, type into, or depend on visually.
---

# Frontend For OpenClaw

Ship interfaces that hold up in real use, not just static screenshots.

## Process

1. Identify the user flow being changed.
2. Respect the existing design language unless the task explicitly changes it.
3. Build the smallest complete interaction slice first.
4. Verify layout, state changes, and edge conditions.
5. Check the result in a browser when practical.
6. Confirm mobile and desktop sanity for changed surfaces.

## Interface Rules

- Prefer clear hierarchy over decorative complexity.
- Make loading, empty, error, and success states explicit when they matter.
- Preserve accessibility basics: focus order, labels, semantics, and readable contrast.
- Avoid introducing visual churn unrelated to the request.

## Reference Files

Read `references/ui-verification-checklist.md` before closing out user-facing changes.

Read `references/state-surface-checklist.md` when a UI flow adds or changes loading, error, empty, success, or recovery behavior.

Read `references/interaction-regression-checks.md` when the surface looks visually correct but interaction regressions are plausible.

## OpenClaw Guidance

- Use browser-based verification for interaction-heavy changes.
- If a design task is exploratory, keep options structured rather than mixing several directions into one output.
- Separate design judgment from implementation proof: something can look good and still be broken.
