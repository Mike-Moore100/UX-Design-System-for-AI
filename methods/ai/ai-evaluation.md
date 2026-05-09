# AI Evaluation

## What
AI Evaluation defines how an AI feature's output quality, safety, usefulness, and failure modes are measured over time.

AI quality needs continuous evidence.

## Why it matters
AI output quality can drift with prompts, models, retrieval data, and user behaviour.

Good evaluation:
- improves output quality
- catches regressions
- supports safer iteration
- reveals common failure modes
- connects model behaviour to user outcomes

Without evaluation, AI features become opinion-led.

## When to apply
- AI assistants
- agents
- retrieval systems
- summarisation
- generation
- recommendation
- classification
- prompt or model changes

## How to apply

- define quality criteria for the task
- create representative test cases
- include edge cases and failure cases
- track user corrections, retries, rejects, and accepts
- evaluate retrieval quality when sources are used
- review high-risk outputs before expanding automation

The team should know whether the AI feature is getting better or worse.

## Implementation rules

- AI feature must have task-specific quality criteria
- representative examples must be tested before major changes
- user feedback signals must be captured where useful
- model, prompt, and retrieval changes must be evaluated
- high-risk outputs need stronger review
- evaluation must include failure and refusal quality

## Example

Bad:
- ships prompt change based on one good demo
- no tracking of rejected outputs
- retrieval answers cite irrelevant sources
- evaluation ignores failure cases

Good:
- test set for common tasks
- accept/edit/retry signals tracked
- retrieval source quality checked
- prompt changes compared against baseline

## Fail conditions

- no definition of good output exists
- model changes are untested
- user corrections are invisible
- failure cases are ignored
- output quality cannot be compared over time

## Enforcement rule

If an AI feature affects user outcomes, define evaluation criteria and feedback signals before scaling it.

