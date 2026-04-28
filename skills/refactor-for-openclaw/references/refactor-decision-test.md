# Refactor Decision Test

Use this before broad structural edits.

## Good Reasons To Refactor

- repeated logic is causing real maintenance cost
- a module interface is harder to understand than the behavior warrants
- testing is difficult because responsibilities are tangled
- reviewers cannot explain the current structure clearly

## Bad Reasons To Refactor

- the code merely looks old
- you want to rename everything for consistency alone
- you suspect performance gains without measurement
- you are mixing cleanup into unrelated feature work

## Rule

If you cannot name the specific complexity being reduced, the refactor is probably not ready.
