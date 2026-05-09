# Target Size

## What
Target Size ensures interactive controls are large enough to activate accurately with touch, mouse, keyboard, or assistive input.

Small targets create avoidable errors.

## Why it matters
Users have different motor abilities, devices, and contexts.

Good target sizing:
- reduces misclicks
- improves mobile usability
- supports motor accessibility
- increases confidence
- speeds interaction

Easy targets make interfaces feel more reliable.

## When to apply
- buttons
- links
- icon controls
- checkboxes
- radio buttons
- menus
- dense toolbars

## How to apply

- make touch targets at least 44x44px where possible
- keep enough space between controls
- expand hit areas for small icons
- avoid placing destructive actions too close to common actions
- maintain target size across responsive layouts
- provide labels for tiny controls where space allows

The hit area should match user intent, not just visible pixels.

## Implementation rules

- touch targets should be at least 44x44px
- desktop targets should not be smaller than 40x40px for key actions
- spacing between adjacent targets must reduce accidental activation
- icon buttons need adequate padding
- links in paragraphs must be distinguishable and selectable
- target size must not shrink on mobile

## Example

Bad:
- 16px icon button with no padding
- delete beside save with tiny gap
- mobile links too close together

Good:
- padded icon buttons
- separated destructive action
- large primary CTA
- full-row selectable list items where appropriate

## Fail conditions

- users can easily tap the wrong control
- hit area is smaller than visible intent
- controls shrink on mobile
- dense toolbar has no spacing
- destructive action is too close to safe actions

## Enforcement rule

If an action is easy to miss or misactivate, increase target size or spacing.
