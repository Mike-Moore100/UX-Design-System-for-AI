# Experiment Hypothesis

## What
Experiment Hypothesis turns conversion changes into testable statements with a clear reason, audience, metric, and expected effect.

Testing should learn why something works, not only whether numbers moved.

## Why it matters
Random tests create noisy results.

Strong experiment hypotheses:
- improve learning quality
- reduce opinion-led changes
- clarify success metrics
- protect against harmful side effects
- make iteration faster

Without a hypothesis, optimisation becomes guessing.

## When to apply
- A/B tests
- landing page changes
- pricing experiments
- signup flow changes
- email capture tests
- onboarding experiments
- checkout optimisation

## How to apply

- define the audience or traffic segment
- state the observed problem
- explain the behavioural reason for the change
- choose one primary metric
- define guardrail metrics
- set a decision rule before launching
- document what was learned

The test should connect a design change to a user behaviour.

## Implementation rules

- hypothesis must include problem, change, audience, and expected result
- one primary metric must define success
- guardrails must monitor quality, trust, or downstream impact
- variants must isolate the intended change where possible
- test duration and sample requirements must be considered
- do not declare wins from weak or biased data

## Example

Bad:
- "Test a better headline"
- multiple unrelated page changes
- no primary metric
- winner chosen because it feels stronger

Good:
- "For paid search visitors, clarifying setup time in the hero will increase trial starts because it reduces implementation uncertainty."
- primary metric defined
- guardrails tracked
- learning documented

## Fail conditions

- test has no behavioural rationale
- success metric is unclear
- many variables change at once
- results are interpreted without enough data
- downstream harm is ignored

## Enforcement rule

If a conversion change cannot be stated as a testable hypothesis, clarify the hypothesis before running or shipping it.

