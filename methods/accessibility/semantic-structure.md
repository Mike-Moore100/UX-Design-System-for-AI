# Semantic Structure

## What
Semantic Structure uses meaningful HTML, headings, landmarks, labels, and relationships so the interface can be understood by browsers and assistive technology.

Structure is accessibility infrastructure.

## Why it matters
Visual layout alone does not communicate meaning to every user or device.

Strong semantic structure:
- improves screen reader navigation
- supports keyboard users
- improves maintainability
- strengthens SEO on public pages
- reduces ambiguity in complex interfaces

The code structure should match the user-facing structure.

## When to apply
- page layouts
- navigation
- forms
- headings and sections
- tables and data views
- buttons, links, and custom components

## How to apply

- use native elements before ARIA
- keep heading levels logical
- use landmarks for major regions
- associate labels, descriptions, and errors with inputs
- use tables for tabular data
- make links and buttons match their actual behaviour

Users and assistive technology should understand the same structure.

## Implementation rules

- each page should have one clear h1
- heading levels must not jump randomly
- navigation must use nav landmarks where appropriate
- main content must be identifiable
- buttons must perform actions and links must navigate
- ARIA must not override correct native semantics unnecessarily

## Example

Bad:
- all layout built from divs
- headings chosen by visual size only
- links used as buttons
- labels not connected to fields

Good:
- semantic page regions
- logical headings
- native buttons, links, inputs, and tables
- labels and descriptions programmatically connected

## Fail conditions

- assistive technology cannot identify regions or controls
- heading structure is confusing
- form fields have no programmatic labels
- custom elements hide meaning
- visual structure and code structure conflict

## Enforcement rule

If the interface meaning is only visible, rebuild the structure semantically.
