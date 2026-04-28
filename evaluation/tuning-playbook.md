# Trigger Tuning Playbook

Use this playbook when evaluation results show the wrong skill would likely trigger.

## Step 1: Classify the miss

Ask:

- Was the winning skill too broad?
- Was the intended skill too vague or too narrow?
- Was the request naturally ambiguous?
- Do we lack a matching example?
- Does the trigger matrix under-describe the boundary?

## Step 2: Choose the smallest corrective action

### Change the skill description

Do this when the intended skill does not clearly match the way real users ask.

Examples:

- add realistic request phrasing
- sharpen the primary intent
- name the most common developer verbs directly

### Change the trigger matrix

Do this when the skill descriptions are acceptable, but the boundary guidance is under-specified.

Examples:

- add competing trigger examples
- add a missing boundary phrase
- clarify which intent wins when two skills sound plausible

### Add or improve examples

Do this when the repository does not yet reflect common user phrasing.

Examples:

- add a repeated real-world request variant
- add a clearer workflow vs specialist contrast

### Add an ambiguity case

Do this when the request sits on a genuine boundary and could plausibly map to more than one skill.

Examples:

- review vs test
- build vs refactor
- ship vs deploy

## Step 3: Record the change

Whenever you tune the system:

- keep the evaluation result
- update the relevant description, matrix entry, example, or ambiguity case
- add a short revision note explaining why the change was made

## Step 4: Re-check nearby boundaries

A fix for one boundary can make another boundary worse.

Whenever you tune:

- check neighboring skills
- scan ambiguity cases in the same family
- avoid solving one miss by making a description globally broader

## Operating Principle

Prefer narrow, evidence-driven trigger tuning over broad rewrites.
