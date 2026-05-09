# Responsive Composition

## What
Responsive Composition preserves meaning, hierarchy, and usability across screen sizes.

Responsive design is not just resizing.

## Why it matters
Layouts often lose priority when compressed or stretched.

Good responsive composition:
- preserves hierarchy
- protects actions
- improves mobile usability
- prevents overlap
- keeps content readable

The same intent must survive every breakpoint.

## When to apply
- landing pages
- dashboards
- forms
- navigation
- pricing pages
- cards
- complex layouts

## How to apply

- define priority before layout
- stack content in decision order
- preserve primary action visibility
- avoid desktop-only interaction patterns
- set stable dimensions for fixed-format elements
- test narrow, wide, and in-between breakpoints

Responsive layouts should preserve the user path.

## Implementation rules

- primary action must remain visible and usable
- text must not overflow containers
- grids must collapse intentionally
- navigation must remain reachable
- tables need mobile alternatives
- interactive targets must remain large enough

## Example

Bad:
- CTA moves below irrelevant content on mobile
- cards become uneven and confusing
- text overlaps at tablet width

Good:
- mobile stack follows priority
- actions remain close to decisions
- content groups stay intact
- responsive table becomes cards or summary

## Fail conditions

- hierarchy changes accidentally by viewport
- content overlaps or overflows
- primary action becomes hard to find
- layout only works at one size
- mobile experience loses meaning

## Enforcement rule

If a breakpoint changes priority or meaning, rebuild the responsive composition around the user path.
