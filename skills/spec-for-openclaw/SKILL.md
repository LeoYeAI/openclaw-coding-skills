---
name: spec-for-openclaw
description: Define implementation scope before coding inside an OpenClaw workspace. Use when the request sounds like "write a spec", "define this feature first", "clarify scope", "turn this idea into something buildable", or any task where outcome, constraints, interfaces, or acceptance criteria are still fuzzy.
---

# Spec For OpenClaw

Write the implementation target down before code starts.

## Process

1. State the problem in concrete terms.
2. Define the desired outcome from the user's perspective.
3. List constraints from the workspace, runtime, tools, and deployment surface.
4. Identify affected files, systems, and interfaces.
5. Write acceptance criteria that can later be verified.
6. Call out unknowns that must be resolved before broad implementation.

## Output Standard

A useful spec is short, testable, and specific enough that planning becomes straightforward.

Include:

- objective
- scope
- non-goals
- affected surfaces
- acceptance criteria
- verification idea

## Anti-Rationalization

| Rationalization | Response |
|---|---|
| "The task is obvious." | If it is obvious, it should be easy to state clearly. |
| "I can spec while coding." | That usually hides scope drift. Define the target first. |
| "This is just a bug fix." | Bugs still need expected behavior and proof. |
