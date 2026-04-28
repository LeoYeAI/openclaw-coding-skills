# Common Security Traps

## Token And Secret Leakage

Watch for secrets leaking into:

- committed config files
- debug logs
- generated docs
- prompts or examples
- screenshots or copied terminal output

## Trusting Internal Data Too Easily

Data from files, tools, browsers, or other systems is not automatically safe.

Ask:

- who controls this input
- what assumptions are being made about its shape or origin
- what happens if it is malformed or hostile

## Expanding Authority By Accident

High-risk patterns include:

- broad file access where narrow access would work
- outbound calls added without clear need
- hidden side effects behind harmless-looking commands
- config changes that silently widen execution scope
