# Ambiguity Cases

These samples are intentionally hard.

They exist to improve trigger quality where multiple skills could plausibly activate.

## How To Use

- Read the request without looking at the expected answer first.
- Decide which skill you think should trigger.
- Compare against `expected_skill` and `alternatives`.
- If the wrong skill would likely win too often, tighten one or more descriptions.

## Common Boundary Areas

- `build-for-openclaw` vs `refactor-for-openclaw`
- `review-for-openclaw` vs `test-for-openclaw`
- `ship-for-openclaw` vs `deploy-for-openclaw`
- `spec-for-openclaw` vs `plan-for-openclaw`
- `frontend-for-openclaw` vs `debug-for-openclaw`
- `security-for-openclaw` vs `review-for-openclaw`
