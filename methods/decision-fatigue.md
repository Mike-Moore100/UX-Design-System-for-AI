# Decision Fatigue

## What
Decision Fatigue is the decline in decision quality and speed as the number of decisions increases.

The more choices a user makes, the harder each subsequent decision becomes.

## Why it matters
Excessive decisions increase cognitive load, slow users down, and lead to avoidance or poor choices.

Users either:
- delay action
- choose randomly
- abandon the flow entirely

Reducing decisions increases speed, confidence, and completion.

## When to apply
- onboarding flows
- multi-step forms
- configuration-heavy interfaces
- dashboards with many options
- any flow requiring multiple decisions

## How to apply

- reduce the total number of decisions required
- guide users instead of asking them to choose everything
- use defaults to remove unnecessary choices
- group related decisions into simple steps
- delay non-critical decisions until later

Design should minimise thinking at every step.

## Implementation rules

- no more than 1 key decision per step or screen
- use sensible defaults for all optional inputs
- limit visible choices to 3–5 maximum
- avoid presenting all options at once
- break complex flows into smaller guided steps
- remove low-impact or rarely used decisions

## Example

Bad:
- user must configure multiple settings upfront
- many options presented equally
- no guidance on what to choose

Good:
- system pre-selects best options
- user guided step-by-step
- only essential decisions shown first

## Fail conditions

- user delays making a choice
- user abandons mid-flow
- inconsistent or poor decision outcomes
- user feels overwhelmed by options

## Enforcement rule

If the user is making too many decisions, reduce, defer, or automate them until only essential choices remain.
