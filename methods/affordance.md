# Affordance

## What
Affordance is how the design of an element suggests how it should be used.

Users should be able to understand what is clickable, editable, draggable, or interactive without thinking.

## Why it matters
If users cannot immediately tell what actions are possible, they hesitate or make errors.

Poor affordance increases cognitive load, slows interaction, and creates confusion.
Good affordance makes interaction feel obvious and effortless.

## When to apply
- buttons and calls to action
- links and navigation elements
- inputs and form fields
- interactive components (cards, lists, toggles)
- any element that requires user interaction

## How to apply

- make interactive elements visually distinct from static content
- use familiar patterns (buttons look like buttons, links look like links)
- apply visual cues such as shape, contrast, and spacing
- ensure hover, focus, and active states reinforce interactivity
- avoid ambiguous elements that look clickable but are not

Interaction should be understood instantly, without instruction.

## Implementation rules

- buttons must have clear visual styling (background, border, or elevation)
- links must be visually distinguishable (color, underline, or consistent pattern)
- clickable areas must be large enough (minimum 40x40px)
- interactive elements must have visible hover, focus, and active states
- do not rely on color alone to indicate interactivity
- ensure consistent styling across all similar elements

## Example

Bad:
- text that looks clickable but is not
- clickable elements styled the same as static content
- no hover or interaction feedback

Good:
- clearly styled buttons with contrast
- links visually distinct from text
- interactive elements respond to hover and click

## Fail conditions

- user does not know what is clickable
- user misses interactive elements
- user clicks non-interactive elements expecting a response
- inconsistent interaction patterns across the UI

## Enforcement rule

If a user has to guess whether something is interactive, the affordance has failed - make interaction obvious through design.
