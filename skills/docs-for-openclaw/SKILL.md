---
name: docs-for-openclaw
description: Update technical documentation, operational notes, prompts, or decision records in an OpenClaw workspace with the same rigor used for code. Use when the request sounds like "update the docs", "write this down", "capture this decision", "document the setup", or when behavior changes and future agents need durable written context instead of tribal knowledge.
---

# Docs For OpenClaw

Write the minimum documentation that prevents future confusion.

## Process

1. Identify what changed and who needs the knowledge.
2. Prefer updating the closest existing document over adding a new random file.
3. Explain behavior and decisions, not just mechanics.
4. Keep instructions aligned with what was actually verified.
5. Remove or correct stale guidance when you find it.

## Documentation Rules

- Document why when the reason is not obvious from the code.
- Keep setup or operational steps concrete.
- Do not describe states that no longer exist.
- If a rule is important enough to repeat often, encode it into a skill or durable reference.

## OpenClaw Guidance

- Use `AGENTS.md`, `TOOLS.md`, daily memory, and project-local docs for durable context when appropriate.
- Do not put sensitive tokens, secrets, or private data into reusable docs.
- Prefer documentation that helps future agents act correctly without re-discovering the same lesson.
