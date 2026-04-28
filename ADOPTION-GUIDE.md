# Adoption Guide

This guide helps teams choose how much of the repository to adopt.

## Option 1: Minimal Workflow Layer

Use this when you want better engineering discipline with minimal context overhead.

Recommended set:

- `openclaw-dev-workflow`
- `plan-for-openclaw`
- `build-for-openclaw`
- `test-for-openclaw`
- `review-for-openclaw`
- `ship-for-openclaw`

Best for:

- general coding assistance
- teams that want better process without many specialist rules
- environments sensitive to context size

## Option 2: Workflow Plus High-Risk Specialists

Add:

- `debug-for-openclaw`
- `security-for-openclaw`
- `deploy-for-openclaw`

Best for:

- production-facing products
- teams with frequent incident, auth, config, or rollout risk
- engineering work where failure cost is non-trivial

## Option 3: Full Engineering Stack

Add all skills in the repository.

Best for:

- larger codebases
- teams with frequent UI work and ongoing refactors
- environments where stronger behavior shaping matters more than minimal context size

## Selection Rule

Start smaller if you are unsure. Expand the stack when repeated task types justify more specialist guidance.
