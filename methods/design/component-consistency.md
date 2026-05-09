# Component Consistency

## What
Component Consistency means similar interface elements look, behave, and respond the same way across the product.

Consistency builds trust.

## Why it matters
Inconsistent components make users relearn the interface.

Strong consistency:
- improves predictability
- reduces cognitive load
- speeds up interaction
- makes the product feel higher quality
- prevents accidental misuse

## When to apply
- buttons
- forms
- navigation
- cards and panels
- modals and drawers
- empty, loading, error, and success states

## How to apply

- reuse existing components before creating new ones
- keep variants limited and purposeful
- use consistent spacing, radius, borders, and states
- make similar actions look similar
- make different-risk actions visually distinct
- preserve interaction feedback across components

Users should not need to relearn controls from screen to screen.

## Implementation rules

- primary, secondary, destructive, and disabled states must be visually distinct
- similar components must share the same structure
- state styles must be consistent across the product
- component variants must have a clear reason to exist
- do not create one-off styling for a single screen unless the interaction truly requires it
- maintain accessible focus, hover, active, and disabled states

## Example

Bad:
- primary buttons use different colours on different screens
- form fields have inconsistent spacing and focus states
- cards change padding and radius without purpose
- destructive actions look like normal actions

Good:
- clear component variants
- predictable states
- reused layout patterns
- consistent spacing and interaction feedback

## Fail conditions

- similar actions look different
- different actions look the same
- users cannot predict what a component will do
- states are missing or inconsistent
- visual variants multiply without purpose

## Enforcement rule

If a component breaks an established pattern without improving clarity or usability, align it with the system.
