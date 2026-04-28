# Behavior Preservation Checks

## Before Refactor

- state what behavior must remain unchanged
- identify the most fragile paths
- identify what existing proof already exists

## During Refactor

- verify after each meaningful structural change
- watch for subtle interface drift
- avoid assuming unchanged behavior just because tests still compile

## After Refactor

- re-check the original critical paths
- inspect whether naming or structure changes introduced confusion elsewhere
- confirm the code is clearer, not merely rearranged

## Rule

A refactor is only successful if complexity goes down and confidence does not.
