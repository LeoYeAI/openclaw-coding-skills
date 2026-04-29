# Release Notes

## Version 1.0.0

**OpenClaw Coding Skills — First Public Release**

A complete coding behavior system for OpenClaw agents, part of the MyClaw.ai ecosystem.

### What's Included

**13 Skills**
- 7 workflow skills: `spec` → `plan` → `build` → `test` → `review` → `ship` + `openclaw-dev-workflow`
- 6 specialist skills: `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor`

**21 Execution References**
- Reusable decision scaffolding inside high-risk skills
- Covers failure patterns, triage loops, rollback strategies, trust boundaries, slice patterns, and more

**131-Rule Trigger Matrix**
- Request-to-skill mapping with boundary guidance
- Designed to improve automatic skill selection quality

**39 Evaluation Samples**
- Labeled trigger-evaluation datasets across 6 files
- Includes ambiguity cases for boundary-case analysis

**Full Tuning Infrastructure**
- Tuning playbook, result schema, feedback loop
- Dry-run validation with recorded results
- Live validation framework with feedback-to-repo playbook

**9 Language READMEs**
- English, 中文, Deutsch, Français, Español, Italiano, 日本語, Русский, Português

**MyClaw.ai Ecosystem Integration**
- Detailed ecosystem section with links to guardian, auto-dream, backup, and bench projects
- Powered by MyClaw.ai badge and positioning throughout

### Architecture

```
openclaw-coding-skills/
├── skills/           13 skills with SKILL.md + references/
├── evaluation/       39 samples, 6 datasets, validation & tuning infrastructure
├── examples/         realistic request samples for trigger calibration
├── README.md         + 8 language variants
├── QUICKSTART.md     shortest path from install to first validation
├── INSTALL.md        minimal adoption guide
├── ADOPTION-GUIDE.md skill-set combinations by team need
└── project.json      machine-readable project metadata
```

### Practical Outcome

This repository provides four layers of improvement for OpenClaw coding sessions:

1. **Better default behavior** — skills shape agent decisions at the right points
2. **Stronger execution support** — references reduce guesswork during high-risk tasks
3. **Better automatic triggering** — trigger matrix and examples improve skill selection
4. **Repeatable tuning** — evaluation, live validation, and feedback loop make the system improvable over time

---

## Version 0.3.0 (pre-release)

Internal development milestone. Turned the repository from a basic skill collection into a structured coding-optimization system.

## Version 0.2.0 (pre-release)

Initial skill set with basic trigger matrix and evaluation samples.
