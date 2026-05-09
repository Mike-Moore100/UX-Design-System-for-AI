# Error Identification

## What
Error Identification ensures users can notice, understand, and fix errors without confusion.

Accessible errors must be visible, descriptive, and programmatically connected to the relevant field or action.

## Why it matters
Unclear errors block completion and disproportionately harm users relying on assistive technology.

Good error identification:
- explains what went wrong
- tells users how to fix it
- preserves entered data
- announces important failures
- reduces repeated mistakes

Errors should guide recovery, not punish the user.

## When to apply
- forms
- checkout
- account setup
- authentication
- destructive actions
- any task with validation or failure states

## How to apply

- place errors near the relevant field
- provide an error summary for complex forms
- describe the problem and solution
- associate errors programmatically with fields
- avoid colour-only error states
- preserve user input after failure

The user should know exactly what to fix and where to fix it.

## Implementation rules

- invalid fields must have text-based error messages
- errors must be linked with inputs using accessible relationships
- error summaries must be focusable when used
- colour must not be the only error indicator
- validation should happen at the right time, not too early
- successful recovery must be clearly confirmed

## Example

Bad:
- "Invalid input"
- red border only
- form clears after failure
- error appears far from the field

Good:
- "Password must be at least 12 characters"
- error text beside the field
- error linked to the input
- focus moves to summary after failed submission

## Fail conditions

- user cannot identify which field failed
- error does not explain how to fix it
- error is not announced or reachable
- user input is lost
- error state relies on colour alone

## Enforcement rule

If an error does not help the user recover, rewrite and reconnect the error state.
