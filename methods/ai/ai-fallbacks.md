# AI Fallbacks

## What
AI Fallbacks define what happens when an AI feature is slow, unavailable, uncertain, refuses, or produces unusable output.

AI failure should not trap the user.

## Why it matters
AI systems fail in more varied ways than deterministic software.

Good fallbacks:
- preserve user progress
- reduce frustration
- keep critical tasks usable
- explain failure without blame
- support retry and manual alternatives

An AI feature that fails silently feels unreliable.

## When to apply
- AI generation
- AI agents
- summarisation
- search and retrieval
- recommendations
- extraction
- classification
- automation

## How to apply

- identify likely AI failure modes
- provide retry, edit, manual, or alternate paths
- preserve user input and partial output
- explain refusals or uncertainty clearly
- avoid infinite loading or vague errors
- degrade gracefully for non-critical AI features

The user should always have a next step.

## Implementation rules

- slow AI calls must show progress or status
- failures must explain recovery
- user inputs must be preserved
- refusals must be clear and useful
- manual fallback must exist for critical tasks
- partial results must be labelled if incomplete

## Example

Bad:
- AI generation fails and clears the prompt
- refusal says only "Cannot complete"
- agent gets stuck with no cancel option
- critical workflow depends entirely on AI uptime

Good:
- retry with preserved input
- manual edit path
- clear refusal explanation
- partial result labelled
- fallback form for critical task

## Fail conditions

- user loses work
- failure has no recovery path
- AI loading never resolves
- refusal is vague
- critical task cannot proceed without AI

## Enforcement rule

If AI can fail, design the recovery path before shipping the feature.

