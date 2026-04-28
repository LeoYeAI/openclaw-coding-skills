---
name: security-for-openclaw
description: Apply practical application-security discipline to coding work in an OpenClaw workspace. Use when the request sounds like "is this secure", "review auth", "we are touching tokens or secrets", "this code handles user input", "this calls an external API", or any task that expands trust boundaries.
---

# Security For OpenClaw

Treat every trust boundary as real.

## Process

1. Identify inputs, outputs, and privilege boundaries.
2. List which surfaces accept untrusted data.
3. Check where secrets, tokens, or credentials might flow.
4. Validate assumptions about auth, authorization, and file access.
5. Reduce permissions and exposure where possible.
6. Verify the change does not create a broader attack surface than needed.

## OpenClaw-Specific Focus

- Distinguish internal workspace actions from external side effects.
- Avoid leaking secrets into commits, logs, prompts, or generated docs.
- Be careful with browser automation and external fetches when they cross trust boundaries.
- Prefer explicit user approval for risky outbound or destructive actions.
- Treat tool invocation power as part of the security model, not just the application code.

## Reference Files

Read `references/trust-boundary-checklist.md` when a task crosses file, network, auth, or execution boundaries.

Read `references/common-traps.md` when the task touches secrets, tokens, external APIs, logs, prompts, or configuration.

Read `references/review-prompts.md` when doing a focused security review and you need sharper inspection questions.

## Review Questions

- Can untrusted input cross a boundary without validation?
- Can a token or secret be exposed through code, logs, or config?
- Does the change broaden file, network, or execution authority?
- Is the new behavior safe by default?
