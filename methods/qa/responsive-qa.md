# Responsive QA

## What
Responsive QA verifies that a screen works across the viewport sizes, density, input modes, and layout constraints users are likely to use.

Responsive quality means the task still works, not only that the layout shrinks.

## Why it matters
Many AI-built interfaces break at real breakpoints.

Responsive QA:
- prevents overlap and clipping
- protects primary actions
- improves mobile usability
- catches density problems
- preserves design consistency

If the layout breaks on common screens, the product is not production-ready.

## When to apply
- any user-facing UI
- dashboards
- navigation
- forms
- pricing pages
- modals
- tables
- toolbars

## How to apply

- test common mobile, tablet, laptop, and wide desktop widths
- check primary actions remain visible and usable
- verify text wraps without overlap
- inspect fixed controls, sticky areas, and modals
- test touch targets on touch layouts
- confirm content order still matches user priority

The user should be able to complete the task at every supported size.

## Implementation rules

- text must not overflow or overlap
- primary actions must remain reachable
- fixed elements must not cover content
- tables or dense layouts must have a usable small-screen strategy
- modals must fit within the viewport
- breakpoints must be verified against realistic content

## Example

Bad:
- pricing cards overflow on mobile
- sticky footer covers form errors
- dashboard table becomes unreadable
- modal actions disappear below the viewport

Good:
- cards stack with clear hierarchy
- sticky UI preserves content space
- dense tables adapt or scroll intentionally
- modal content and actions remain reachable

## Fail conditions

- critical content is clipped
- actions are hidden or unreachable
- layout overlaps at common breakpoints
- touch targets become too small
- content order no longer supports the task

## Enforcement rule

If a supported viewport prevents task completion, fix the responsive behaviour before release.

