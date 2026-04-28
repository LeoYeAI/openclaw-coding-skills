---
name: openclaw-dev-workflow
description: Enforce a production-grade development workflow for OpenClaw coding work. Use when the request is broad or end-to-end, such as "build this feature", "fix this properly", "handle this coding task", "implement this across the codebase", or "help me ship this safely", especially when work spans multiple files and needs planning, verification, and clean closeout.
---

# OpenClaw Dev Workflow

Use this skill to orchestrate coding work end to end inside an OpenClaw workspace.

This is the default workflow layer. Pair it with narrower domain skills when a task needs frontend, security, performance, deployment, or framework-specific depth.

## Core Rules

- Read the local workspace contract before major work.
- Let local rules override generic habits.
- Create or update `plan.md` for long tasks when required.
- Prefer first-class OpenClaw tools over improvised shell-heavy flows.
- Verify before claiming completion.
- End with a clean git commit unless told not to.

## Workflow

### 1. Frame

- Classify the task.
- Determine risk and breadth.
- Decide whether direct execution or a staged plan is appropriate.

### 2. Gather context

- Read only the files needed for the current slice.
- Search for existing patterns before inventing new ones.
- Retrieve prior context when historical decisions matter.

### 3. Execute in slices

- Pick the smallest meaningful increment.
- Implement it.
- Verify it.
- Update the task plan.

### 4. Close out

- Review the final diff.
- Update any required docs.
- Commit.
- Report evidence and residual risk.

## Reference Files

Read when needed:

- `references/task-shapes.md`
- `references/verification-matrix.md`
- `references/git-closeout.md`
