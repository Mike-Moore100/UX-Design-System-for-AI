# Data Minimisation

## What
Data Minimisation means collecting, storing, and exposing only the data needed for a clear purpose.

Less unnecessary data means less risk.

## Why it matters
Extra data increases breach impact, privacy risk, compliance burden, and user distrust.

Data minimisation:
- reduces exposure
- improves trust
- simplifies permissions
- lowers operational risk
- supports privacy expectations

If data is not needed, do not collect it.

## When to apply
- signup
- profiles
- analytics
- forms
- exports
- admin views
- integrations

## How to apply

- ask why each field is needed
- defer optional data collection
- avoid exposing full records when summaries suffice
- limit retention where possible
- redact sensitive values in UI and logs
- make data use understandable

The product should collect data with purpose.

## Implementation rules

- required fields must be justified
- optional fields must be clearly optional
- sensitive data must not appear unnecessarily
- exports should include only requested data
- logs must avoid unnecessary personal data
- retention should match product need

## Example

Bad:
- phone number required for newsletter signup
- full customer record shown in every admin view
- logs store personal details unnecessarily

Good:
- email-only signup when enough
- masked sensitive fields
- scoped exports
- clear reason for required data

## Fail conditions

- data is collected without clear purpose
- sensitive data appears where not needed
- optional data is treated as required
- logs contain unnecessary personal data
- retention is indefinite without reason

## Enforcement rule

If data is not necessary for the task or product purpose, do not collect or expose it.
