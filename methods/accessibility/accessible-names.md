# Accessible Names

## What
Accessible Names are the programmatic labels assistive technologies use to identify controls and interactive elements.

Every control needs a clear name.

## Why it matters
Screen reader and voice control users rely on accessible names to understand and operate interfaces.

Good accessible names:
- explain control purpose
- support voice commands
- reduce ambiguity
- improve form usability
- make icon-only controls usable

If a control has no name, many users cannot use it.

## When to apply
- buttons
- links
- form fields
- icon-only controls
- menus
- dialogs
- custom components

## How to apply

- use visible text labels where possible
- connect labels to inputs programmatically
- give icon-only buttons clear accessible labels
- avoid duplicate names for different actions
- keep names concise and specific
- ensure accessible names match visible labels where possible

The accessible name should answer "what is this control?"

## Implementation rules

- every interactive element must have an accessible name
- icon-only controls need aria-label or equivalent text
- labels must be associated with inputs
- visible and accessible labels must not conflict
- repeated controls need context where necessary
- decorative icons must be hidden from assistive technology

## Example

Bad:
- button labelled only with an unlabeled icon
- multiple links named "Read more"
- input with placeholder but no label

Good:
- "Search projects"
- "Delete invoice April 2026"
- visible label connected to field

## Fail conditions

- assistive technology announces "button" with no name
- multiple controls have indistinguishable names
- accessible label conflicts with visible text
- placeholder is used as the only label
- icon meaning is not exposed

## Enforcement rule

If a control cannot be identified by assistive technology, add a clear accessible name before shipping.
