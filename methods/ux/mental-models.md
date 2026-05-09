# Mental Models

## What
Mental Models are the expectations users bring from prior experience about how something should work.

Interfaces should match the user's model or carefully teach a new one.

## Why it matters
Users act based on what they believe will happen.

Matching mental models:
- reduces learning effort
- improves predictability
- prevents errors
- increases confidence
- makes new products feel familiar

Breaking expectations creates friction unless the improvement is obvious.

## When to apply
- navigation
- settings
- dashboards
- forms
- AI workflows
- data models
- new product categories

## How to apply

- identify what users already expect
- use familiar structures for common tasks
- name concepts in user language
- show cause and effect clearly
- introduce new models gradually
- avoid surprising behaviour without explanation

The interface should behave the way users reasonably expect.

## Implementation rules

- labels must match user concepts
- object relationships must be clear
- actions must produce predictable results
- new concepts need examples or onboarding
- destructive and reversible actions must behave consistently
- do not use internal system architecture as the user model

## Example

Bad:
- "workspace" and "project" mean different things across screens
- deleting an item archives it sometimes and removes it other times
- AI controls use internal model jargon

Good:
- consistent object names
- predictable action outcomes
- examples for new concepts
- product structure matches user workflow

## Fail conditions

- user expects one result and gets another
- product terms conflict with user terms
- same action behaves differently across contexts
- model is based on implementation, not user reality
- new concepts are introduced without support

## Enforcement rule

If the user's expectation and system behaviour differ, align the interface or explain the difference before action.
