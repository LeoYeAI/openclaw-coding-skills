---
name: plan-for-openclaw
description: Break coding work into ordered, verifiable tasks for OpenClaw execution. Use when the request sounds like "make a plan", "break this into steps", "split this into tasks", "figure out the implementation order", or when work spans enough files or uncertainty that explicit checkpointing and a maintained plan file will reduce risk.
---

# Plan For OpenClaw

Convert intent into a sequence the agent can execute without losing rigor.

## Process

1. Read the relevant local rules.
2. Decide whether the task qualifies as a long task.
3. Create or update `plan.md` when the workspace requires it.
4. Break the work into thin vertical slices.
5. Order slices by dependency and risk.
6. Define what evidence will mark each slice complete.
7. Keep the plan updated during execution.

## Planning Heuristics

- Prefer tasks that can be verified independently.
- Avoid steps that combine refactor, feature work, and cleanup in one block.
- Put the highest-uncertainty slice early enough to de-risk the task.
- Keep wording operational, not aspirational.

## Red Flags

- A task list that is really just a vague summary
- Large steps with no verification story
- A plan that stops being updated after work begins
