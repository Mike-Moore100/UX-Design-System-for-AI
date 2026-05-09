# Spacing Rhythm

## What
Spacing Rhythm is the consistent use of space to group related elements, separate unrelated elements, and create a calm reading flow.

Whitespace is structure.

## Why it matters
Poor spacing makes interfaces feel cluttered even when the content is simple.

Strong spacing:
- clarifies grouping
- improves scanning
- reduces cognitive load
- makes actions easier to find
- increases perceived quality

## When to apply
- forms
- cards and panels
- dashboards
- navigation
- content sections
- any repeated component system

## How to apply

- use a consistent spacing scale
- keep related items close together
- separate unrelated groups with larger spacing
- use spacing before borders when grouping can be solved with whitespace
- align spacing across repeated components
- avoid random one-off gaps

The user should feel the structure without needing extra dividers.

## Implementation rules

- spacing must follow the product scale
- parent-child relationships must be visible through proximity
- repeated components must use consistent internal spacing
- sections must have more spacing between them than items inside them
- interactive elements need enough space to avoid accidental activation
- reduce visual density before adding decoration

## Example

Bad:
- equal spacing between everything
- cramped controls
- unrelated groups appear connected
- repeated cards use different internal padding

Good:
- tight spacing inside groups
- larger spacing between groups
- consistent component padding
- clear scan path from content to action

## Fail conditions

- relationships between elements are unclear
- screen feels dense or noisy
- spacing changes without purpose
- controls are too close together
- user has to search for group boundaries

## Enforcement rule

If spacing does not explain structure, adjust proximity and rhythm before adding visual styling.
