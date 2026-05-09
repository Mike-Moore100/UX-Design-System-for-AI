# Contrast Minimums

## What
Contrast Minimums ensure text, controls, focus indicators, and meaningful graphics are readable and distinguishable.

Contrast protects perception.

## Why it matters
Low contrast blocks users with low vision, glare, poor displays, or temporary visual strain.

Good contrast:
- improves readability
- supports focus visibility
- protects state recognition
- improves mobile use
- increases confidence

Readable design is a baseline requirement.

## When to apply
- text
- buttons
- form fields
- icons
- charts
- focus states
- disabled and muted states

## How to apply

- check text contrast against backgrounds
- keep muted text readable
- make focus indicators visible
- avoid colour-only state differences
- test light and dark themes
- ensure non-text controls have visible boundaries

Contrast should support hierarchy without sacrificing readability.

## Implementation rules

- normal text must meet WCAG contrast targets
- large text still needs adequate contrast
- focus indicators must be visible
- icons conveying meaning need sufficient contrast
- disabled text should not contain essential information
- charts must not rely on low-contrast colours

## Example

Bad:
- light grey body text on white
- blue and purple lines with no labels
- invisible focus ring

Good:
- readable muted text
- high-contrast focus outline
- labelled chart series
- clear button boundaries

## Fail conditions

- text is hard to read
- state relies on subtle colour shift
- focus cannot be seen
- chart values are indistinguishable
- dark mode reduces readability

## Enforcement rule

If contrast prevents perception or recognition, increase contrast before considering the design complete.
