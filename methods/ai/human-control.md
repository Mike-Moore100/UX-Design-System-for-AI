# Human Control

## What
Human Control keeps users in charge of AI-assisted actions, especially when changes are irreversible, public, costly, or sensitive.

AI should assist the decision, not silently take it away.

## Why it matters
Automation without control creates risk and distrust.

Human control:
- preserves agency
- prevents unwanted actions
- supports accountability
- reduces automation surprises
- improves trust in AI features

Users must be able to understand and interrupt important AI actions.

## When to apply
- AI agents
- automation workflows
- content publishing
- code changes
- financial actions
- customer messages
- admin tasks
- destructive actions

## How to apply

- define which actions require review
- show what the AI plans to do before it acts
- allow pause, cancel, edit, and approve
- separate suggestions from executed actions
- require confirmation for irreversible or external actions
- keep an audit trail for important automation

The user should know what the AI will do and be able to stop it.

## Implementation rules

- high-impact AI actions must require human approval
- AI plans must be visible before execution when stakes are meaningful
- cancel or pause must be available for long-running automation
- external sends, deletes, purchases, and permission changes must be confirmed
- action history must be available for review
- automation must fail safe when uncertain

## Example

Bad:
- AI emails customers without preview
- agent deletes records automatically
- user cannot stop a long-running task
- AI changes permissions silently

Good:
- AI drafts, user approves
- plan preview before execution
- cancel button during run
- confirmation for irreversible actions
- audit trail of completed steps

## Fail conditions

- AI executes high-impact actions without review
- user cannot interrupt automation
- plan is hidden
- action history is missing
- unsafe action is the default

## Enforcement rule

If an AI action affects other people, money, access, production data, or public content, require visible human control.

