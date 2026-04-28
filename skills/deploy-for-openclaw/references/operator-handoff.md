# Operator Handoff

## Minimum Handoff Content

Include:

- what is changing
- what environment assumptions exist
- what manual steps are required
- what success looks like after rollout
- what symptoms indicate immediate rollback or investigation

## Bad Handoffs

- "just deploy it"
- "should be fine"
- hidden config dependencies
- no mention of startup checks or user-path verification

## Rule

If another operator cannot execute the rollout safely from your handoff, the handoff is incomplete.
