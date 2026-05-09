# Typography

## What
Typography is the use of type size, weight, line height, and spacing to make content readable and scannable.

Type must create clarity before personality.

## Why it matters
Users scan before they read.

Poor typography causes:
- slow comprehension
- weak hierarchy
- crowded layouts
- reduced trust

Strong typography creates:
- clear reading order
- faster scanning
- better comprehension
- more confident action

## When to apply
- headings and page titles
- forms and labels
- product copy
- navigation
- cards, tables, and dashboards
- any screen with dense information

## How to apply

- use size, weight, and spacing to create a clear reading order
- keep body text comfortable to read
- use short line lengths for long-form content
- use labels and helper text with enough visual separation
- avoid making too many elements bold
- do not use oversized type inside compact UI surfaces

Users should understand the content structure before reading every word.

## Implementation rules

- every screen needs one dominant text element
- headings must be visually distinct from body text
- body text must have comfortable line height
- labels must be close to the controls they describe
- muted text must remain readable
- type scale must be consistent across similar components

## Example

Bad:
- all text uses similar size and weight
- headings are too large for the container
- muted text is unreadable
- dense paragraphs block scanning

Good:
- clear heading, supporting copy, and label hierarchy
- readable body text
- compact UI text sized to its container
- consistent type scale across screens

## Fail conditions

- user cannot tell what to read first
- text feels cramped
- supporting copy competes with headings
- labels or helper text are hard to associate with controls
- text hierarchy changes randomly across screens

## Enforcement rule

If typography does not make the screen easier to scan and understand, simplify the type scale and strengthen the hierarchy.
