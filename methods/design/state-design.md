# State Design

## What
State Design defines how components and screens communicate normal, hover, focus, active, loading, disabled, success, warning, and error states.

States are part of the interface contract.

## Why it matters
Missing or inconsistent states make products feel unresponsive and unreliable.

Good state design:
- confirms interaction
- prevents uncertainty
- supports accessibility
- communicates system status
- improves trust

Every interactive element needs clear states.

## When to apply
- buttons
- inputs
- cards
- navigation
- menus
- modals
- async actions

## How to apply

- define states for each component
- make focus visible
- show loading immediately
- distinguish disabled and loading states
- confirm success or failure
- keep state styling consistent

Users should always know what is interactive and what changed.

## Implementation rules

- hover must not be the only interaction feedback
- focus state must be visible
- loading state must prevent duplicate submission when needed
- disabled state must explain why when unclear
- success and error states must be visually distinct
- state styles must not shift layout unexpectedly

## Example

Bad:
- button click has no response
- disabled button looks like normal button
- focus ring removed

Good:
- immediate pressed state
- loading spinner with disabled repeat action
- visible focus
- success confirmation

## Fail conditions

- user cannot tell if action worked
- interactive state is invisible
- focus is hidden
- loading allows accidental duplicate actions
- states differ randomly across components

## Enforcement rule

If a component can change or be interacted with, define and display its states consistently.
