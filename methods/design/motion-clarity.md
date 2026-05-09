# Motion Clarity

## What
Motion Clarity is the use of animation to explain change, confirm action, and guide attention.

Motion must improve understanding.

## Why it matters
Bad motion slows users down, distracts attention, and makes the product feel unstable.

Good motion:
- confirms interaction
- explains state changes
- supports perceived performance
- guides attention
- makes transitions feel predictable

## When to apply
- hover, focus, and active states
- loading and progress states
- menus, drawers, and modals
- form validation
- success and completion moments
- screen or section transitions

## How to apply

- use motion to show cause and effect
- keep timing fast and restrained
- animate only the elements involved in the state change
- avoid decorative looping motion in task surfaces
- respect reduced motion preferences
- make feedback immediate

Motion should make the interface feel clearer, not busier.

## Implementation rules

- micro interactions should feel immediate
- standard transitions should be short and predictable
- loading states must appear quickly
- animations must not block task completion
- motion must not hide important information
- reduced motion alternatives must preserve meaning

## Example

Bad:
- decorative animations compete with the primary action
- slow transitions delay interaction
- state changes happen without visible feedback
- motion draws attention away from the task

Good:
- button press gives immediate feedback
- drawer movement explains where content came from
- loading state appears quickly
- success motion confirms completion

## Fail conditions

- motion delays the user
- animation exists only for decoration
- state changes are unclear
- reduced motion users lose meaning
- movement distracts from the primary action

## Enforcement rule

If motion does not clarify feedback, state, or direction, remove it or reduce it.
