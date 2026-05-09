# Performance Budget

## What
Performance Budget sets limits for page weight, loading time, interaction delay, and expensive work before the interface becomes slow.

A budget turns performance from a vague goal into a constraint.

## Why it matters
Products become slow one small addition at a time.

Performance budgets:
- protect critical journeys
- prevent bundle and asset creep
- make tradeoffs explicit
- improve reliability on slower devices
- keep teams honest before launch

Without a budget, performance regressions feel accidental until users leave.

## When to apply
- landing pages
- dashboards
- checkout flows
- onboarding
- data-heavy pages
- mobile-first products
- media-rich interfaces

## How to apply

- define the critical user journey
- set limits for JavaScript, CSS, images, fonts, and API work
- prioritise first useful render over decorative assets
- defer non-critical work
- remove unused dependencies or heavy components
- measure before and after changes when possible

The budget should protect what the user needs first.

## Implementation rules

- critical routes must have explicit weight or timing targets
- non-critical scripts must not block first useful render
- large dependencies must justify their value
- images and fonts must be budgeted
- performance regressions must be treated as product regressions
- budget exceptions must be documented

## Example

Bad:
- adds a charting library for one small chart
- loads all dashboard modules before the first screen
- ships large images without compression
- accepts slower load because the UI looks richer

Good:
- route-level bundle limits
- lazy-loaded secondary modules
- compressed responsive images
- measured impact before release

## Fail conditions

- page weight grows without review
- primary journey slows after visual additions
- non-critical work blocks user action
- no one can explain the performance target
- regressions are accepted silently

## Enforcement rule

If a change makes the critical journey slower, reduce cost or justify the tradeoff with measurable user value.

