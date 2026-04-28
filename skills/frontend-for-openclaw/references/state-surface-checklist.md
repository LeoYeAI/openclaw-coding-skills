# State Surface Checklist

## Check All Meaningful States

For any changed UI flow, ask whether these states are covered where relevant:

- initial state
- loading state
- success state
- empty state
- error state
- retry or recovery state

## Common Failure Pattern

A UI can look finished in the happy path while still being broken in the states users actually hit under stress.

## Rule

If the code change introduces a new user path, make sure the state surface is not silently incomplete.
