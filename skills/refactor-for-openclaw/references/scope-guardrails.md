# Scope Guardrails

## Keep Refactor Scope Honest

Good refactor scope:

- one module or one structural concern at a time
- one class of duplication at a time
- one interface simplification at a time

Bad refactor scope:

- cleanup plus feature work mixed together
- cleanup plus renaming plus architecture rewrite in one pass
- touching every adjacent file because the code feels inconsistent

## Rule

If the explanation of the refactor starts needing several paragraphs, the scope is probably too wide.
