# WCAG POUR

## What
WCAG POUR is the accessibility model that requires interfaces to be Perceivable, Operable, Understandable, and Robust.

It is the foundation of modern accessibility standards.

## Why it matters
Users access products with different abilities, devices, assistive technologies, and contexts.

POUR helps ensure:
- content can be perceived
- controls can be operated
- information can be understood
- implementation works with assistive technology

Accessibility must be designed into the screen, not added after.

## When to apply
- all user-facing screens
- forms and flows
- navigation
- interactive components
- public pages
- any task with legal, financial, health, or account impact

## How to apply

- make content available through more than one sense
- ensure every action is keyboard-operable
- use clear labels, instructions, and error messages
- use semantic HTML and stable component patterns
- avoid custom controls unless accessibility behaviour is complete
- validate the experience against real interaction states

Users should be able to perceive, operate, understand, and rely on the interface.

## Implementation rules

- every meaningful image needs useful alt text or empty alt if decorative
- every control must be keyboard accessible
- every form field needs a programmatic label
- state must be communicated without colour alone
- semantic HTML must be preferred over generic elements
- custom components must expose correct roles, names, values, and states

## Example

Bad:
- clickable divs with no keyboard support
- icon-only actions with no accessible name
- errors shown only in red
- form labels as placeholders only

Good:
- semantic buttons and links
- visible and programmatic labels
- state communicated through text, icons, and ARIA where needed
- keyboard and screen reader paths preserved

## Fail conditions

- user cannot complete the flow with keyboard
- assistive technology cannot identify controls
- meaning depends on colour alone
- form errors are unclear or unannounced
- custom components do not expose correct state

## Enforcement rule

If a screen fails Perceivable, Operable, Understandable, or Robust, it must be fixed before it is production-ready.
