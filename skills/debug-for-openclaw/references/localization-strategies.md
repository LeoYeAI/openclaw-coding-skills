# Localization Strategies

## Narrow By Boundary

Ask which layer first exhibits the failure:

- input parsing
- business logic
- persistence
- external integration
- UI interaction
- deployment/runtime wiring

## Narrow By Time

Ask when the failure first appeared:

- after a specific commit
- after a refactor
- after config change
- after dependency update
- only under repeated execution

## Narrow By Condition

Ask what changes the outcome:

- valid vs invalid input
- one environment vs another
- cold start vs warm state
- single run vs repeated run

## Rule

A good debugging step reduces the search space. If it does not, it is probably noise.
