# Funnel Instrumentation

## What
Funnel Instrumentation measures how users move through a multi-step journey and where they drop off.

Funnels should reveal friction, not only count completions.

## Why it matters
Conversion and activation problems often hide between screens.

Good funnel instrumentation:
- identifies abandonment points
- clarifies step performance
- supports prioritisation
- helps compare variants
- reveals unintended friction

Without funnel data, teams optimise the loudest opinion.

## When to apply
- signup
- onboarding
- checkout
- lead capture
- trial activation
- account setup
- upgrade flows
- booking flows

## How to apply

- define the start, steps, and success event
- track meaningful step completion and abandonment
- include source or segment where useful
- capture error states that block progress
- define guardrail metrics like support requests or refunds
- avoid counting vanity page views as progress

The funnel should show where users lose momentum and why.

## Implementation rules

- funnel steps must match real user decisions
- success event must represent meaningful completion
- events must fire once per real action
- drop-off points must be observable
- error and validation blockers should be tracked when relevant
- segment properties must be useful and privacy-aware

## Example

Bad:
- tracks only page views
- start and completion events use inconsistent identifiers
- errors are invisible in analytics
- checkout success fires before payment succeeds

Good:
- `signup_started`
- `workspace_created`
- `invite_step_skipped`
- `checkout_completed`
- validation failures tracked without sensitive input values

## Fail conditions

- funnel cannot show where users abandon
- events fire multiple times for one action
- success metric is not real success
- key blockers are invisible
- tracking collects unnecessary personal data

## Enforcement rule

If a flow matters to the business or user activation, instrument the journey from intent to completion.

