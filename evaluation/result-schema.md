# Evaluation Result Schema

Use this schema when recording how a trigger evaluation actually behaved.

## Fields

### `sample_id`

Stable id from one of the evaluation files.

### `request`

The evaluated request text.

### `expected_skill`

The skill the repository currently believes should be the primary trigger.

### `actual_skill`

The skill that would actually trigger, or did trigger, under the current descriptions.

### `matched`

Boolean value.

- `true` when `actual_skill` matches `expected_skill`
- `false` when it does not

### `validation_strength`

Optional qualitative field for manual validation.

Suggested values:

- `clear`
- `borderline`
- `weak`

### `failure_reason`

Use when `matched` is `false`.

Suggested values:

- `description-too-broad`
- `description-too-narrow`
- `boundary-confusion`
- `missing-example`
- `missing-ambiguity-case`
- `matrix-mismatch`
- `other`

### `revision_note`

Short note describing what should change next.

## Example

```json
{
  "sample_id": "amb-003",
  "request": "Before we merge this, tell me what proof is still missing.",
  "expected_skill": "test-for-openclaw",
  "actual_skill": "review-for-openclaw",
  "matched": false,
  "validation_strength": "borderline",
  "failure_reason": "boundary-confusion",
  "revision_note": "Make test-focused proof language more prominent in test-for-openclaw description."
}
```
