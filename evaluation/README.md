# Evaluation

This directory contains trigger-evaluation samples for the skill system.

The purpose is to test whether realistic developer requests would likely activate the intended skill.

## Format

Samples are stored as JSONL.

Each line contains:

- `id`: stable sample id
- `request`: realistic user request text
- `expected_skill`: the most likely skill that should activate
- `category`: `workflow`, `specialist`, or `ambiguity`
- `notes`: short explanation of why the mapping exists
- `alternatives`: optional array for plausible competing skills in ambiguity cases

## How To Use

- Compare an incoming real request to these samples.
- Check whether the currently configured trigger descriptions would likely select the expected skill.
- If many ambiguous cases appear, refine skill descriptions, trigger matrix entries, or example tasks.
- Add new samples whenever repeated real phrasing shows up in actual usage.

## Files

- `workflow.jsonl`
- `specialist.jsonl`
- `ambiguity.jsonl`
- `ambiguity-notes.md`
- `result-schema.md`
- `results-template.jsonl`
- `tuning-playbook.md`
- `VALIDATION-RUN-001.md`
- `validation-run-001-results.jsonl`
- `VALIDATION-SUMMARY.md`
- `LIVE-VALIDATION.md`
- `live-results-template.jsonl`
- `live-run-template.md`
- `live-feedback-playbook.md`
- `tuning-log-template.md`
