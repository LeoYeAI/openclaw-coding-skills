# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/skills-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![References](https://img.shields.io/badge/execution_references-21-green?style=for-the-badge)](./skills/)
[![Eval Samples](https://img.shields.io/badge/eval_samples-39-orange?style=for-the-badge)](./evaluation/)
[![Trigger Rules](https://img.shields.io/badge/trigger_matrix-131_rules-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![License](https://img.shields.io/badge/license-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMTAiIGN5PSIxMCIgcj0iOCIgZmlsbD0id2hpdGUiLz48L3N2Zz4=)](https://myclaw.ai)

**Stop hoping the agent gets it right. Start making reliable coding behavior the default.**

[中文说明](./README.zh-CN.md)

---

### At a Glance

| Layer | What It Contains | Count |
|-------|-----------------|-------|
| **Workflow Skills** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **Specialist Skills** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **Execution References** | Reusable decision scaffolding inside high-risk skills | 21 files |
| **Trigger Matrix** | Request-to-skill mapping with boundary guidance | 131 rules |
| **Evaluation Assets** | Labeled samples, ambiguity cases, dry-run & live validation | 39 samples across 6 datasets |
| **Tuning Infrastructure** | Playbook, result schema, feedback loop, tuning log templates | Full closed-loop |

> **70+ files · 13 skills · 21 execution references · 39 eval samples · 131 trigger rules**

---

Production-grade coding skills for OpenClaw agents.

Part of the [MyClaw.ai](https://myclaw.ai) ecosystem: a growing set of open assets designed to turn raw agent capability into dependable software execution.

## About MyClaw.ai

[MyClaw.ai](https://myclaw.ai) is an AI personal assistant platform that gives every user a full server running [OpenClaw](https://github.com/openclaw/openclaw) — the leading open-source AI agent framework. Each MyClaw instance comes with complete code control, networking, tool access, and the ability to install skills like this one.

Within the MyClaw.ai ecosystem, this repository serves as the **coding behavior layer**: it bridges the gap between "the model can write code" and "the agent can execute software work with discipline." MyClaw users can install these skills directly into their instance to immediately improve coding session quality.

The MyClaw.ai open ecosystem includes:

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — structured coding behavior system (this repo)
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — security monitoring and protection
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — cognitive memory consolidation
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — full instance backup and restore
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — agent capability benchmarking

All open-source. All designed to make AI agents more capable, more reliable, and more useful in real work.

---

This project gives OpenClaw a structured coding behavior layer for real development work. It helps agents scope tasks more clearly, execute in smaller and safer slices, verify more rigorously, and close work with stronger engineering discipline across feature work, bug fixing, refactoring, review, and shipping.

## What This Project Is

OpenClaw agents are powerful, but raw capability alone does not reliably produce high-quality coding behavior. Good coding outcomes depend on repeatable habits: better scoping, better sequencing, better verification, and stronger closeout discipline.

This repository provides that missing layer.

Within the MyClaw.ai ecosystem, it serves as a coding behavior system for OpenClaw: reusable workflow skills, specialist skills, execution references, trigger guidance, and evaluation assets that help teams move from "the model can code" to "the agent can execute software work with discipline."

The core logic is straightforward:

- raw model capability is not enough
- behavior quality is shaped at decision points
- skills improve those decision points
- references reduce guesswork during execution
- evaluation and live validation make the system tunable over time

The result is not a smarter base model. The result is a more reliable coding agent.

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

## Why This Matters

Most agent failures in software work do not come from lack of raw intelligence. They come from weak execution habits.

Agents fail because they:

- start coding before the task is scoped clearly
- make large changes without controlling blast radius
- declare success on weak evidence
- blur boundaries between implementation, testing, review, and deployment
- handle high-risk tasks with too little structure

This repository is designed to reduce exactly those failures.

It helps an OpenClaw agent:

- choose better task boundaries before editing
- move in smaller, more defensible slices
- verify with stronger evidence before claiming completion
- debug by reducing uncertainty instead of stacking guesses
- review changes with clearer risk articulation
- handle refactors and deployments with less silent risk

The value is not theoretical. The value is a higher-quality default execution pattern for real coding sessions.

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

Good engineering discipline should not depend on whether the current agent session happens to be careful.

The best human engineers are not the ones who occasionally write great code. They are the ones whose worst day still meets a high bar. These skills exist to give OpenClaw agents that same property: a reliable floor, not just a high ceiling.
