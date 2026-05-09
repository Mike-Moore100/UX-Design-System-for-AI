# Fitts’s Law

## What
The time required to interact with a target depends on its size and distance.  
Larger, closer targets are faster and easier to use.

## Why it matters
Small or distant targets increase effort and error rates.  
Poor targeting slows users down, causes misclicks, and reduces confidence.

Good targeting:
- speeds up interaction
- reduces errors
- improves flow and usability

## When to apply
- buttons and primary actions
- navigation (top bars, sidebars, menus)
- forms and inputs
- mobile interfaces
- any clickable or tappable element

## How to apply

- make primary actions large and easy to hit
- position key actions within natural reach (thumb zones on mobile, central focus on desktop)
- increase spacing between interactive elements
- avoid placing critical actions in edges or hard-to-reach areas
- prioritise accessibility for all interaction methods

Interaction should feel fast and effortless.

## Implementation rules

- minimum target size: 40x40px (desktop), 44x44px recommended (mobile)
- primary actions must be larger than secondary actions
- maintain adequate spacing between clickable elements (minimum 8–12px)
- avoid placing primary actions near edges where misclicks occur
- ensure consistent positioning of key actions across screens
- reduce distance between related actions when used together

## Example

Bad:
- small buttons placed close together
- primary action hard to reach or locate
- crowded clickable areas causing errors

Good:
- large, clearly defined primary button
- well-spaced interactive elements
- key actions placed in predictable, easy-to-reach locations

## Fail conditions

- missed or inaccurate clicks
- slow interaction speed
- accidental clicks on nearby elements
- user struggles to reach or locate key actions

## Enforcement rule

If an action is small, hard to reach, or easy to miss, it must be resized or repositioned until interaction is fast and reliable.
