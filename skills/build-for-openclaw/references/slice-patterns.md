# Slice Patterns

## Small Feature Slice

Use this pattern when adding new behavior with low architectural risk.

1. define the smallest user-visible outcome
2. identify the minimum files that must change
3. implement only that path
4. verify the new path narrowly
5. stop and reassess before expanding scope

## Bug Fix Slice

1. reproduce the failure
2. identify the smallest code surface that can remove it
3. patch only that surface
4. verify the failure no longer occurs
5. add a guard where practical

## Refactor Slice

1. define the behavior that must remain stable
2. simplify one structural unit at a time
3. verify after each meaningful step
4. avoid mixing feature changes into the slice

## Expansion Rule

If a slice starts touching unrelated concerns, stop and split it.
