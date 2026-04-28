# Installation

## Option 1: Copy selected skills

Copy one or more folders from `skills/` into your OpenClaw skill collection.

Recommended minimum set:

- `openclaw-dev-workflow`
- `plan-for-openclaw`
- `build-for-openclaw`
- `test-for-openclaw`
- `review-for-openclaw`
- `ship-for-openclaw`

## Option 2: Use the whole repository as a skill source

Keep this repository in your workspace and reference the skill folders directly from your OpenClaw setup.

## Adoption Guidance

- Start with the workflow layer first.
- Add specialist skills only when they map to real task frequency.
- Avoid loading every skill by default if your environment is context-sensitive.

## Suggested First Validation

After installing, trigger a multi-file coding task and confirm the agent:

- creates or updates `plan.md` for long work
- verifies before claiming success
- closes with clean handoff discipline
