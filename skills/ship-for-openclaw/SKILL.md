---
name: ship-for-openclaw
description: Prepare an OpenClaw change for safe handoff or release. Use when the request sounds like "wrap this up", "close this out", "are we ready to ship", "prepare final handoff", or any task where work is complete enough to need a disciplined final pass over diffs, verification, documentation, and rollout risk.
---

# Ship For OpenClaw

Finish with discipline.

## Process

1. Re-read the final diff with accidental change detection in mind.
2. Confirm the requested outcome is actually met.
3. Confirm verification matches the risk of the change.
4. Update docs, prompts, or operational notes if behavior changed.
5. Create a focused git commit unless the user said not to.
6. Summarize outcome, evidence, and residual risk.

## Closeout Rules

- Do not hide unverified areas.
- Do not include unrelated churn in the final diff.
- Do not claim deploy safety without a concrete basis.
- Prefer one coherent commit over a messy pile of saves.
