# Zoom and Reflow

## What
Zoom and Reflow ensure content remains usable when users zoom, enlarge text, or use narrow viewports.

Accessibility must survive magnification.

## Why it matters
Many users enlarge content to read comfortably.

Good reflow:
- prevents horizontal scrolling
- preserves task order
- keeps controls reachable
- improves mobile usability
- protects readability

Zoom should make the interface easier, not broken.

## When to apply
- all responsive layouts
- forms
- dashboards
- tables
- navigation
- modals
- content pages

## How to apply

- use responsive layouts
- avoid fixed heights that clip text
- allow text to wrap
- preserve focus and reading order
- provide alternatives for wide tables
- test zoom and text enlargement

The layout should adapt without hiding meaning.

## Implementation rules

- text must not be clipped at larger sizes
- content must reflow at narrow widths
- controls must remain visible and usable
- horizontal scrolling should be avoided except for true data tables
- modals must fit small viewports
- order must remain logical after reflow

## Example

Bad:
- enlarged text overlaps buttons
- fixed modal cannot scroll
- table forces full-page horizontal scrolling

Good:
- flexible containers
- wrapped labels
- scrollable modal content
- table summary or card layout on small screens

## Fail conditions

- zoom hides content
- text overlaps or clips
- primary action moves out of reach
- reading order breaks
- modal traps content offscreen

## Enforcement rule

If zoom or narrow layout breaks the task, rebuild the layout to reflow predictably.
