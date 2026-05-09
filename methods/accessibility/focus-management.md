# Focus Management

## What
Focus Management controls where keyboard and assistive technology attention moves after interactions, route changes, errors, and overlays.

Focus is the user's location in the interface.

## Why it matters
Poor focus management makes interfaces feel broken for keyboard and screen reader users.

Strong focus management:
- preserves orientation
- explains state changes
- supports recovery
- makes dynamic interfaces usable

Focus should move only when it helps the user continue.

## When to apply
- modals and dialogs
- route changes
- form validation
- dynamic content updates
- menus and popovers
- multi-step flows

## How to apply

- keep visible focus indicators clear
- move focus to newly opened dialogs
- return focus when overlays close
- move focus to important error summaries
- avoid stealing focus during normal typing or reading
- ensure route changes announce a new context

The user should always know where they are and what changed.

## Implementation rules

- focus styles must be visible and high contrast
- focus must enter modals when they open
- focus must return to the trigger when modals close
- validation errors must be reachable and associated with fields
- route changes should set focus to the page heading or main region
- dynamic updates must not unexpectedly interrupt the user

## Example

Bad:
- focus disappears after closing a modal
- validation errors appear above the form but focus stays hidden
- page changes but screen reader remains in the old context
- focus ring is removed for aesthetics

Good:
- strong visible focus state
- modal focus trap with return focus
- error summary receives focus when submission fails
- route changes orient the user to the new page

## Fail conditions

- focus is invisible
- focus moves unexpectedly
- focus does not move when context changes
- user loses their place after closing an overlay
- errors are not reachable from the keyboard path

## Enforcement rule

If focus behaviour causes disorientation, restore predictable focus before shipping the interaction.
