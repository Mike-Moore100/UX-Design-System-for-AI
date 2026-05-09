# Experiment Measurement

## What
Experiment Measurement defines how product tests are tracked, evaluated, and interpreted.

Experiments should create decision-quality evidence.

## Why it matters
Poor experiment measurement creates false winners and wasted work.

Strong measurement:
- clarifies primary outcomes
- protects guardrail metrics
- improves learning quality
- prevents cherry-picking
- supports confident rollout decisions

Testing without measurement discipline is expensive guessing.

## When to apply
- A/B tests
- pricing tests
- onboarding changes
- landing pages
- checkout changes
- feature rollouts
- AI output experiments

## How to apply

- define one primary metric before launch
- define guardrail metrics
- ensure variants are assigned consistently
- track exposure separately from conversion
- avoid changing the test midstream without noting it
- document the decision and learning after the test

The experiment should answer a specific product question.

## Implementation rules

- every experiment must have a hypothesis
- exposure event must be tracked
- primary metric must be defined before launch
- guardrails must protect trust, quality, and downstream impact
- sample and duration limitations must be acknowledged
- results must be interpreted against the original hypothesis

## Example

Bad:
- test starts without a primary metric
- winner chosen from whichever metric improved
- exposure is not tracked
- rollout ignores increased support tickets

Good:
- hypothesis documented
- exposure and conversion events tracked
- guardrails include activation and refunds
- learning recorded before rollout

## Fail conditions

- no primary metric exists
- assignment or exposure is unreliable
- guardrail metrics are missing
- results are cherry-picked
- test changes are not documented

## Enforcement rule

If an experiment cannot be measured against a pre-defined decision rule, do not treat it as evidence.

