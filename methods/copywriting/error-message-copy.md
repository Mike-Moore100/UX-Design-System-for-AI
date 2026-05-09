# Error Message Copy

## What
Error Message Copy explains what went wrong, why it matters when useful, and how the user can recover.

Errors should help users regain control.

## Why it matters
Poor error copy creates frustration and abandonment.

Good error copy:
- reduces confusion
- supports accessibility
- improves task completion
- lowers support burden
- preserves trust during failure

The user should never have to guess what to do next.

## When to apply
- forms
- payments
- uploads
- authentication
- settings
- destructive actions
- network failures
- permissions issues

## How to apply

- state the problem in plain language
- identify the affected field or action
- explain recovery steps
- preserve user input where possible
- avoid blame
- provide support or retry paths for unresolved errors

The message should turn failure into a clear next step.

## Implementation rules

- error must be specific
- recovery action must be visible
- message must be close to the affected control where possible
- copy must not expose sensitive technical details
- user input must not be erased unnecessarily
- repeated failures must offer an alternate path

## Example

Bad:
- "Invalid"
- "Error 500"
- "You entered the wrong information"
- "Something went wrong" with no next step

Good:
- "Enter a valid email address, like name@example.com"
- "We could not process the payment. Check the card details or use another card."
- "Upload a PNG or JPG under 5 MB"

## Fail conditions

- user cannot tell what failed
- recovery is unclear
- copy blames the user
- sensitive system details are exposed
- error appears far from the problem

## Enforcement rule

If an error message does not help the user recover, rewrite it before changing error styling.

