# OpenClaw Coding Skills

[中文说明](./README.zh-CN.md)

Production-grade coding skills for OpenClaw agents.

Part of the MyClaw.ai ecosystem: a growing set of open assets that help teams get more reliable output from agent-driven coding and software development.

This project provides a structured execution system for software development inside OpenClaw workspaces. It is designed to improve consistency, verification discipline, task breakdown, and release safety across feature work, bug fixing, refactoring, review, and shipping.

## What This Project Is

OpenClaw agents are powerful, but raw capability alone does not guarantee strong engineering outcomes. This repository encodes reusable workflows so coding sessions follow a higher bar by default.

Within the MyClaw.ai ecosystem, this repository plays the role of a coding behavior layer: it helps turn raw agent capability into more disciplined execution, stronger verification habits, and a tunable workflow system that teams can improve over time.

The project is built around a simple idea:

- define work clearly
- break it into small slices
- implement with evidence
- verify before claiming success
- close with clean diffs and scoped commits

## Skill Set

Core workflow skills:

- `spec-for-openclaw`
- `plan-for-openclaw`
- `build-for-openclaw`
- `test-for-openclaw`
- `review-for-openclaw`
- `ship-for-openclaw`
- `openclaw-dev-workflow`

Specialist skills:

- `debug-for-openclaw`
- `security-for-openclaw`
- `frontend-for-openclaw`
- `docs-for-openclaw`
- `deploy-for-openclaw`
- `refactor-for-openclaw`

Support materials live under `references/` inside each skill when needed. These references are part of the performance strategy: they give the agent reusable execution patterns instead of only abstract advice.

## Design Goals

- Fit OpenClaw's tool model instead of generic CLI assumptions
- Respect workspace-local operating rules like `AGENTS.md`
- Prefer evidence-based completion over optimistic completion
- Keep skills modular so teams can adopt one or the whole set
- Stay tool-agnostic at the skill layer while remaining OpenClaw-native in execution guidance

## Why This Improves Coding Performance

These skills do not change the base model itself. They improve coding performance by changing agent behavior at the right decision points.

They are designed to make an OpenClaw agent:

- choose better task boundaries before editing
- verify more often and with more appropriate evidence
- debug by reducing uncertainty instead of stacking guesses
- review changes with stronger finding structure
- handle refactors and deployments with less silent risk

The practical effect is not "smarter model weights". The practical effect is more reliable engineering behavior.

## Repository Layout

```text
openclaw-coding-skills/
├── README.md
├── README.zh-CN.md
├── examples/
├── evaluation/
└── skills/
```

## Usage

Install the skills into an OpenClaw skill directory, or copy the specific skill folders you want into your own workspace skill collection.

See [QUICKSTART.md](./QUICKSTART.md) for the shortest path from install to first real-task validation.

See [INSTALL.md](./INSTALL.md) for a minimal adoption path and first-run validation guidance.

See [ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md) for recommended skill-set combinations based on team needs and context budget.

See [skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md) for request-to-skill mapping used to improve automatic trigger quality.

See [examples/README.md](./examples/README.md) for realistic request examples used to calibrate trigger quality over time.

See [evaluation/README.md](./evaluation/README.md) for labeled trigger-evaluation samples that support iterative tuning.

See [evaluation/ambiguity.jsonl](./evaluation/ambiguity.jsonl) for hard boundary cases where multiple skills could plausibly trigger.

See [evaluation/tuning-playbook.md](./evaluation/tuning-playbook.md) and [evaluation/result-schema.md](./evaluation/result-schema.md) for the trigger-tuning feedback loop.

See [evaluation/VALIDATION-SUMMARY.md](./evaluation/VALIDATION-SUMMARY.md) for the first practical dry-run validation of the repository.

See [evaluation/LIVE-VALIDATION.md](./evaluation/LIVE-VALIDATION.md) and [evaluation/live-results-template.jsonl](./evaluation/live-results-template.jsonl) for real-task validation recording.

See [evaluation/live-feedback-playbook.md](./evaluation/live-feedback-playbook.md) and [evaluation/tuning-log-template.md](./evaluation/tuning-log-template.md) for turning live-task observations into repository updates.

See [VERSIONING.md](./VERSIONING.md), [RELEASE-NOTES.md](./RELEASE-NOTES.md), and [PUBLISHING.md](./PUBLISHING.md) for release-oriented repository management.

See [REPO-METADATA.md](./REPO-METADATA.md) for suggested public repo description, topics, and positioning.

See [FINAL-PUBLISH-CHECKLIST.md](./FINAL-PUBLISH-CHECKLIST.md) for the last pre-publish review pass.

See [MAINTENANCE-BOUNDARY.md](./MAINTENANCE-BOUNDARY.md) for guidance on when the repository is already good enough and what to improve next.

Recommended adoption order:

1. `openclaw-dev-workflow`
2. `plan-for-openclaw`
3. `build-for-openclaw`
4. `test-for-openclaw`
5. `review-for-openclaw`
6. `ship-for-openclaw`
7. Add specialist skills based on your codebase risk profile: `debug-for-openclaw`, `security-for-openclaw`, `frontend-for-openclaw`, `docs-for-openclaw`, `deploy-for-openclaw`, `refactor-for-openclaw`

## Philosophy

Good engineering discipline should not depend on whether the current agent session happens to be careful. These skills make rigor more repeatable.
