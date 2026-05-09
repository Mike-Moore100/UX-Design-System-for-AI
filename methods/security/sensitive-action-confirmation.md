# Sensitive Action Confirmation

## What
Sensitive Action Confirmation adds deliberate friction before irreversible, destructive, expensive, or high-risk actions.

Not all friction is bad.

## Why it matters
Fast interfaces can make dangerous mistakes easier.

Good confirmation:
- prevents accidental harm
- makes consequences clear
- supports informed consent
- reduces support burden
- protects trust

Sensitive actions need clarity before completion.

## When to apply
- deleting data
- changing billing
- removing users
- changing permissions
- publishing private content
- exporting sensitive data
- disabling security settings

## How to apply

- explain the consequence in plain language
- show what will be affected
- require confirmation proportional to risk
- avoid generic "Are you sure?" dialogs
- provide undo when possible
- require re-authentication for high-risk account changes

The user should understand the impact before the action completes.

## Implementation rules

- destructive buttons must be clearly labelled
- irreversible actions must describe consequences
- high-risk actions must not be one-click unless undo is reliable
- confirmation copy must name the object being affected
- dangerous actions must be visually distinct from normal actions
- success and failure states must be explicit

## Example

Bad:
- "Are you sure?"
- delete button beside normal actions
- no explanation of what will be lost
- permission downgrade with no warning

Good:
- "Delete Project Alpha and its 12 files"
- clear consequence copy
- typed confirmation for critical deletion
- undo for recoverable changes

## Fail conditions

- user can trigger irreversible harm accidentally
- confirmation does not explain impact
- dangerous action looks normal
- object or scope is unclear
- no recovery path exists for preventable mistakes

## Enforcement rule

If an action can cause serious harm, slow it down until the user understands the consequence.
