# Tesler's Law

## What
Tesler's Law states that every system has inherent complexity, and that complexity must be handled either by the system or by the user.

Good UX absorbs complexity where possible.

## Why it matters
Pushing system complexity onto users creates confusion, errors, and abandonment.

Managing complexity:
- reduces user effort
- improves task completion
- makes advanced tools approachable
- prevents configuration overload
- increases trust

The product should not make users manage complexity the system can handle.

## When to apply
- setup flows
- configuration screens
- dashboards
- AI tools
- advanced settings
- imports and integrations
- enterprise workflows

## How to apply

- automate predictable decisions
- provide sensible defaults
- progressively reveal advanced controls
- explain unavoidable complexity clearly
- split complex tasks into meaningful steps
- preserve expert control without overwhelming beginners

Complexity should appear only when the user is ready for it.

## Implementation rules

- required setup must be minimal
- advanced options must not block first value
- defaults must be safe and useful
- complex states must have clear summaries
- automation must allow review when risk is high
- do not hide complexity that changes outcomes materially

## Example

Bad:
- user must configure every setting before starting
- advanced options shown before the core task
- AI output requires unexplained manual cleanup

Good:
- quick start with defaults
- advanced controls behind disclosure
- summary before committing complex changes
- smart defaults inferred from context

## Fail conditions

- user must understand internal system complexity
- setup blocks value
- advanced options overwhelm simple tasks
- defaults are unsafe or poor
- hidden complexity causes surprising outcomes

## Enforcement rule

If complexity can be handled by the system without harming trust, move it out of the user's way.
