# Privacy Aware Analytics

## What
Privacy Aware Analytics measures product behaviour while minimising personal data collection and respecting consent requirements.

Analytics should earn user trust.

## Why it matters
Measurement can create privacy, legal, and brand risk when it collects too much.

Privacy-aware analytics:
- reduces data exposure
- supports compliance
- improves user trust
- limits blast radius
- keeps teams focused on useful metrics

More data is not always better data.

## When to apply
- public websites
- signup flows
- healthcare, finance, or sensitive products
- AI prompt logging
- session replay
- product analytics
- third-party tracking

## How to apply

- collect the minimum data needed for a decision
- avoid sending sensitive input values
- respect consent and regional requirements
- anonymise, aggregate, or hash where appropriate
- define retention expectations
- review third-party analytics scripts for risk

The team should be able to learn without over-collecting.

## Implementation rules

- sensitive personal data must not be tracked by default
- analytics properties must have a clear purpose
- consent requirements must be respected
- AI prompts and outputs must not be logged casually
- session replay must mask sensitive fields
- retention and access should match actual need

## Example

Bad:
- logs full form fields into analytics
- records AI prompts containing customer data
- adds session replay without masking
- tracks every click with no purpose

Good:
- tracks step completion without raw field values
- masks sensitive inputs
- separates product metrics from personal data
- documents analytics purpose and retention

## Fail conditions

- analytics collects unnecessary personal data
- consent is ignored
- sensitive AI inputs are logged without policy
- third-party scripts create hidden exposure
- retention is undefined

## Enforcement rule

If analytics does not need personal or sensitive data to answer the decision, do not collect it.

