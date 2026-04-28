# Specialist Examples

## `debug-for-openclaw`

Most likely trigger for requests like:

- This test started failing and I do not know why.
- The build broke after my last change.
- It only fails in one path and I cannot localize it.
- Help me debug this instead of guessing fixes.
- The logs are noisy but the root cause is still unclear.

## `security-for-openclaw`

Most likely trigger for requests like:

- Review this auth flow for security issues.
- We are touching secrets and external APIs here, check the risk.
- Is this safe to ship from a trust-boundary perspective?
- This code handles user input and file access, inspect it carefully.
- Tell me whether this change expands permissions too far.

## `frontend-for-openclaw`

Most likely trigger for requests like:

- Build this settings screen.
- Fix this broken interaction in the browser flow.
- Make this page responsive without redesigning the whole app.
- Update this component and verify it still works on mobile.
- This UI looks fine in code review but broken in actual use.

## `docs-for-openclaw`

Most likely trigger for requests like:

- Update the docs to match this behavior change.
- Write down the new setup steps.
- Capture this architecture decision so future agents stop re-learning it.
- Document the operational workflow we just changed.
- Clean up stale instructions in this project.

## `deploy-for-openclaw`

Most likely trigger for requests like:

- Prepare this for production rollout.
- What is the rollback plan for this config change?
- We need to deploy this safely.
- Check release readiness before we touch prod.
- This affects runtime wiring, treat it like a deployment risk.

## `refactor-for-openclaw`

Most likely trigger for requests like:

- Clean this module up without changing behavior.
- Reduce duplication in this service.
- This code works, but it is getting too hard to maintain.
- Refactor this carefully and keep the interfaces stable.
- Simplify this logic so future changes are less painful.
