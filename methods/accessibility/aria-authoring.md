# ARIA Authoring

## What
ARIA Authoring uses roles, states, and properties to make custom components understandable to assistive technology.

ARIA should repair gaps, not replace native HTML.

## Why it matters
Incorrect ARIA can make an interface less accessible than no ARIA.

Good ARIA:
- exposes custom component meaning
- communicates state
- supports screen reader interaction
- improves complex widgets
- preserves expected patterns

Native HTML should be used first.

## When to apply
- custom dropdowns
- tabs
- accordions
- dialogs
- comboboxes
- menus
- dynamic widgets

## How to apply

- use native elements when possible
- follow established ARIA patterns
- expose role, name, value, and state
- support expected keyboard interaction
- keep ARIA state synced with visual state
- test with assistive technology where possible

ARIA must match actual behaviour.

## Implementation rules

- do not add ARIA that conflicts with native semantics
- custom widgets need complete keyboard support
- expanded, selected, checked, and disabled states must be accurate
- dialogs need labels and focus management
- aria-hidden must not hide focusable content
- live regions must be used sparingly

## Example

Bad:
- div with role button but no keyboard support
- aria-expanded stays false when menu opens
- aria-hidden parent contains focused button

Good:
- native button for button behaviour
- synced expanded state
- labelled dialog with focus trap
- ARIA pattern matching keyboard behaviour

## Fail conditions

- ARIA state is wrong
- custom widget lacks keyboard behaviour
- ARIA overrides useful native semantics
- focusable content is hidden from assistive technology
- component pattern does not match user expectation

## Enforcement rule

If ARIA is used, it must accurately describe behaviour and be paired with complete interaction support.
