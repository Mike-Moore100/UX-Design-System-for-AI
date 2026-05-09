# Iconography

## What
Iconography uses symbols to support recognition, navigation, status, and action.

Icons should clarify, not decorate.

## Why it matters
Icons can speed recognition, but ambiguous icons increase cognitive load.

Good iconography:
- improves scanning
- supports labels
- communicates state
- saves space responsibly
- reinforces familiar patterns

Icons are strongest when meaning is already familiar or labelled.

## When to apply
- navigation
- toolbars
- buttons
- status states
- empty states
- feature lists
- mobile controls

## How to apply

- use familiar icons for common actions
- pair icons with labels when meaning may be unclear
- keep style consistent
- avoid decorative icons in dense task areas
- make status icons accessible with text
- use the same icon for the same concept everywhere

The user should not have to guess what an icon means.

## Implementation rules

- icon-only controls need accessible names
- unfamiliar icons need labels or tooltips
- icons must not be the only state indicator
- icon size and stroke must be consistent
- decorative icons must not compete with actions
- do not reuse one icon for different meanings

## Example

Bad:
- abstract icon-only navigation
- same icon means edit and configure
- status shown only by coloured icon

Good:
- familiar save, search, settings icons
- icon plus label for important navigation
- consistent stroke and size
- state icon with text label

## Fail conditions

- icon meaning is unclear
- icon-only control lacks accessible name
- icons are inconsistent in style
- decorative icons create noise
- same symbol has multiple meanings

## Enforcement rule

If an icon does not improve recognition or state clarity, label it, replace it, or remove it.
