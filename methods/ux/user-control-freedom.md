# User Control and Freedom

## What
User Control and Freedom means users need clear exits, undo paths, cancellation, and recovery from mistakes.

Users should feel in control.

## Why it matters
People make errors and change their minds.

Control and freedom:
- reduces anxiety
- improves confidence
- supports exploration
- prevents abandonment
- reduces support burden

The interface should not trap users.

## When to apply
- modals
- forms
- onboarding
- destructive actions
- checkout
- AI generation flows
- settings changes

## How to apply

- provide cancel and back options
- use undo for reversible actions
- warn before irreversible actions
- preserve work during navigation
- make escape routes visible
- confirm state changes clearly

Users should be able to recover without starting over.

## Implementation rules

- modal close behaviour must be clear
- destructive actions need confirmation or undo
- form progress should be preserved where possible
- back navigation must not lose data unexpectedly
- long processes need cancellation when safe
- generated output should be reviewable before replacing work

## Example

Bad:
- closing modal loses entered data
- irreversible delete happens instantly
- back button breaks a multi-step flow

Good:
- draft is saved
- undo after archive
- confirmation before permanent delete
- clear cancel and return paths

## Fail conditions

- user feels trapped
- mistakes cannot be recovered
- navigation loses work unexpectedly
- cancel behaviour is unclear
- irreversible actions are too easy

## Enforcement rule

If a user can make a mistake, provide a clear way to prevent, cancel, undo, or recover from it.
