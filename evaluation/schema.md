# Evaluation Schema Notes

## Why JSONL

JSONL keeps samples append-only, diff-friendly, and easy to inspect line by line.

## Field Guidance

### `id`

Use stable ids so future discussions can reference exact samples.

### `request`

Write the way a real developer would ask, not the way a taxonomy would label the task.

### `expected_skill`

Choose the single most likely primary skill, even if the real task could later combine with others.

### `notes`

Explain why this mapping exists. Keep it short and operational.
