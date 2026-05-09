# Error Tolerance

## What
Error Tolerance designs systems so user mistakes are prevented, contained, or easy to recover from.

Errors should not become dead ends.

## Why it matters
Users mistype, misunderstand, misclick, and act under pressure.

Error tolerance:
- increases completion
- reduces frustration
- protects trust
- improves accessibility
- lowers support demand

The system should help users succeed despite mistakes.

## When to apply
- forms
- uploads
- checkout
- account settings
- destructive actions
- AI editing flows
- complex workflows

## How to apply

- prevent errors with constraints and defaults
- validate at the right time
- preserve user input
- explain recovery clearly
- provide undo where possible
- make dangerous actions harder than safe actions

The user should know how to recover immediately.

## Implementation rules

- validation must be specific and actionable
- user input must not be lost after failure
- destructive actions need confirmation or undo
- partial success states must be explained
- risky defaults must be avoided
- recovery paths must be visible near the error

## Example

Bad:
- failed upload loses all progress
- checkout error clears the form
- "Invalid" with no explanation

Good:
- invalid field message explains the fix
- failed upload can retry
- checkout preserves entered details
- destructive change can be undone

## Fail conditions

- small mistake causes large damage
- error does not explain recovery
- user must start over
- risky action is too easy
- system blames the user instead of helping

## Enforcement rule

If an error is likely, design prevention and recovery before treating the flow as complete.
