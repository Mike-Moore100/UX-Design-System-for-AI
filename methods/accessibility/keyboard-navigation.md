# Keyboard Navigation

## What
Keyboard Navigation ensures users can move through and operate the interface without a mouse or touch input.

Keyboard access is required for many assistive technologies and power users.

## Why it matters
If a task cannot be completed by keyboard, many users are blocked completely.

Good keyboard navigation:
- supports assistive technology
- improves speed for expert users
- reveals logical interaction order
- prevents trapped or unreachable controls

Keyboard support is a core interaction requirement.

## When to apply
- navigation menus
- forms
- modals and drawers
- dropdowns and comboboxes
- toolbars
- any clickable or focusable element

## How to apply

- use native interactive elements where possible
- keep tab order logical and predictable
- ensure focus never gets trapped unintentionally
- trap focus intentionally inside modals until dismissed
- provide keyboard shortcuts only as enhancements
- make all hover-only content available by keyboard

The keyboard path should match the user's mental path through the screen.

## Implementation rules

- interactive elements must be reachable with Tab
- focus order must follow visual and task order
- Enter and Space must activate controls as expected
- Escape must dismiss temporary overlays when appropriate
- modals must trap focus and return focus on close
- disabled controls must not create confusing focus stops

## Example

Bad:
- custom buttons cannot receive focus
- dropdown only opens on hover
- modal allows focus behind it
- focus order jumps around the page

Good:
- native buttons and links
- predictable tab sequence
- keyboard-operable menus and dialogs
- focus returns to the triggering control

## Fail conditions

- user cannot reach an action by keyboard
- user cannot tell where focus is
- focus becomes trapped accidentally
- modal or menu focus behaviour is broken
- keyboard order does not match the task flow

## Enforcement rule

If a user cannot complete the primary task with a keyboard, the interaction has failed.
