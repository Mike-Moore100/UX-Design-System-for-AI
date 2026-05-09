# Event Taxonomy

## What
Event Taxonomy defines consistent names, properties, and rules for analytics events.

Good analytics starts with language the team can trust.

## Why it matters
Inconsistent event names make product data unreliable.

A strong taxonomy:
- improves analysis quality
- reduces duplicated tracking
- supports funnels and cohorts
- makes dashboards easier to maintain
- prevents teams from arguing over definitions

Bad naming turns analytics into guesswork.

## When to apply
- new product analytics
- funnel tracking
- onboarding
- checkout
- dashboards
- experiments
- feature launches

## How to apply

- define event names around meaningful user actions
- use a consistent naming pattern
- include only useful properties
- document required and optional fields
- avoid tracking the same action under multiple names
- keep product, marketing, and data teams aligned on definitions

The event name should explain what happened without needing code context.

## Implementation rules

- event names must be consistent and human-readable
- events must represent meaningful user or system actions
- properties must support known analysis needs
- personal data must not be collected unless necessary and permitted
- duplicate events must be consolidated
- taxonomy changes must be versioned or documented

## Example

Bad:
- `button_click`
- `ctaClicked`
- `signup_start`
- same action tracked differently across pages

Good:
- `signup_started`
- `plan_selected`
- `checkout_completed`
- consistent properties like `plan`, `source`, and `step`

## Fail conditions

- event names are ambiguous
- same action has multiple event names
- properties are missing for key analysis
- unnecessary sensitive data is tracked
- no shared definition exists

## Enforcement rule

If an event cannot support a clear product decision, rename, redesign, or remove it.

