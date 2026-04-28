---
name: deploy-for-openclaw
description: Prepare and execute deployment-oriented work in an OpenClaw workspace with explicit release safety, environment awareness, and rollback thinking. Use when the request sounds like "deploy this", "prepare this for production", "update config and ship it", "what is the rollback plan", "check release readiness", or when a change could affect production behavior or operator workflow.
---

# Deploy For OpenClaw

Deployments are execution risk, not just a final checkbox.

## Process

1. Confirm what is being deployed and why now.
2. Identify environment-specific assumptions and configuration dependencies.
3. Verify the release candidate with the strongest available pre-deploy evidence.
4. Check what can fail during rollout, startup, migration, or integration.
5. Define rollback or mitigation before treating the change as safe.
6. Communicate readiness, risk, and any required operator steps clearly.

## Deployment Rules

- Do not treat a successful build as a successful deployment.
- Do not hide manual steps or environment dependencies.
- Prefer staged or reversible rollout paths when available.
- Surface monitoring and rollback needs as part of the release story.

## Reference Files

Read `references/release-checklist.md` before high-risk handoff or rollout preparation.

Read `references/rollback-patterns.md` when the change touches config, migrations, runtime wiring, or any path where rollback is not obvious.

Read `references/operator-handoff.md` when another operator may execute or supervise the rollout.

## OpenClaw Guidance

- Treat config changes, gateway actions, and external service wiring as deployment risk.
- If the user did not ask for a live deploy, prepare the path without overstepping into production actions.
- Keep environment notes concrete enough that another operator can execute them.
