# Evidence Ladder

Use the cheapest credible proof that matches the risk.

## Level 1: Diff Review

Use for documentation, prompt wording, or metadata-only changes.

## Level 2: Narrow Runtime Check

Use for local behavior that can be verified through a direct flow or simple execution trace.

## Level 3: Targeted Automated Test

Use for logic changes, bug fixes, and behavior with clear pass/fail conditions.

## Level 4: Multi-Surface Proof

Use when a change affects several layers, such as API plus UI, or config plus runtime behavior.

Combine targeted tests, typecheck, lint, browser verification, or operator checks as needed.

## Rule

If the change could plausibly break user behavior, Level 1 alone is not enough.
