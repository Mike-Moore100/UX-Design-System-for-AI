# Rendering Stability

## What
Rendering Stability prevents unexpected movement, flicker, reflow, and visual instability while content loads or updates.

Stable interfaces feel calmer and more trustworthy.

## Why it matters
Layout shifts cause misclicks, confusion, and perceived poor quality.

Rendering stability:
- improves usability
- prevents accidental actions
- protects reading flow
- supports accessibility
- improves perceived polish

Moving targets make users feel the interface is fighting them.

## When to apply
- feeds
- dashboards
- images
- ads or embeds
- data updates
- responsive layouts
- route changes
- loading states

## How to apply

- reserve dimensions for images, media, embeds, and dynamic modules
- avoid inserting content above the user's current focus unexpectedly
- keep controls in stable positions
- animate state changes only when they aid comprehension
- batch live updates when constant movement would distract
- test narrow and wide layouts for overflow and jumps

The screen should not move unless movement helps the user understand change.

## Implementation rules

- media and embeds must reserve space
- loading placeholders must match final layout
- late-loading content must not push primary actions away
- live updates must not steal focus
- responsive changes must preserve task continuity
- text, controls, and panels must not overlap at breakpoints

## Example

Bad:
- image loads and pushes the CTA down
- toast appears over the primary action
- list updates move the clicked item
- mobile layout overlaps labels and buttons

Good:
- stable reserved image area
- non-blocking status position
- live updates queued or clearly inserted
- responsive constraints prevent overlap

## Fail conditions

- layout shifts cause misclicks
- focus or scroll position changes unexpectedly
- content jumps during loading
- update animation distracts from the task
- breakpoints create overlap

## Enforcement rule

If content changes position unexpectedly during a task, reserve space, reorder updates, or stabilise the layout.

