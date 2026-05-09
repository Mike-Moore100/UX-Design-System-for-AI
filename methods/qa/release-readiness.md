# Release Readiness

## What
Release Readiness determines whether a product change is safe, understandable, measurable, and reversible enough to ship.

Readiness is a product judgment, not just a merge state.

## Why it matters
Good releases balance quality, speed, risk, and learning.

Release readiness:
- prevents avoidable incidents
- clarifies ownership
- ensures monitoring exists
- protects users from incomplete states
- supports rollback or mitigation

Shipping without readiness turns users into testers.

## When to apply
- launches
- pricing changes
- checkout changes
- onboarding changes
- security-sensitive releases
- AI feature releases
- migrations
- major UI changes

## How to apply

- define what must work on release day
- verify critical journeys
- confirm analytics or monitoring exists
- check accessibility, security, and performance risks
- prepare rollback or mitigation where needed
- document known limitations

The team should know what is shipping, why, and how to detect problems.

## Implementation rules

- critical path must be verified
- launch success metric must be defined
- high-risk changes need rollback or mitigation
- known risks must be documented
- monitoring or analytics must cover important outcomes
- user-facing copy must match product reality

## Example

Bad:
- launch has no success metric
- checkout change ships without rollback plan
- AI feature has no failure state
- known mobile issue is not documented

Good:
- critical journeys verified
- monitoring and analytics checked
- rollback path defined
- limitations documented
- support and product copy aligned

## Fail conditions

- no one knows how to tell if release worked
- critical path is unverified
- high-risk change cannot be rolled back
- known risk is hidden
- user-facing claims exceed released capability

## Enforcement rule

If release risk is high and verification is weak, pause, reduce scope, or add mitigation before shipping.

