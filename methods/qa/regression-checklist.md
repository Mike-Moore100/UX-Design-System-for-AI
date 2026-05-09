# Regression Checklist

## What
Regression Checklist protects existing behaviour around the area being changed.

Every change creates risk outside the visible edit.

## Why it matters
Shipping a fix that breaks adjacent behaviour destroys confidence.

Regression checks:
- protect critical flows
- catch unintended side effects
- reduce repeated bugs
- support faster releases
- keep refactors honest

AI-generated edits can easily change more than intended.

## When to apply
- bug fixes
- refactors
- component changes
- navigation changes
- form changes
- design system updates
- shared utility edits

## How to apply

- identify touched components and dependencies
- list adjacent flows likely to be affected
- run existing tests where available
- manually check the critical path when tests are missing
- compare before and after behaviour
- document anything not verified

The checklist should match the blast radius of the change.

## Implementation rules

- shared components require broader checks
- critical flows must be tested after related edits
- existing user behaviour must not change accidentally
- skipped checks must be stated
- screenshots or visual checks should be used for UI risk
- regression tests should be added when a bug is likely to return

## Example

Bad:
- changes button component and checks only one page
- refactors form validation without testing errors
- fixes mobile nav and breaks desktop keyboard focus
- no note about unverified flows

Good:
- changed component impact listed
- critical paths tested
- relevant automated tests run
- residual risk documented

## Fail conditions

- adjacent flow breaks
- shared component impact is ignored
- old bug can return easily
- no verification evidence exists
- skipped checks are hidden

## Enforcement rule

If a change touches shared behaviour, verify the likely affected flows before release.

