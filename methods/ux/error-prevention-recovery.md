# Error Prevention and Recovery

## What
Error Prevention focuses on stopping mistakes before they happen.  
Error Recovery ensures users can easily fix issues when they occur.

## Why it matters
Errors break flow, increase frustration, and reduce trust.

Without proper handling, users:
- get stuck
- abandon tasks
- lose confidence

Good error design keeps users moving forward.

## When to apply
- forms and inputs
- multi-step processes
- critical user actions
- data entry and validation

## How to apply

- prevent errors through constraints and guidance
- validate inputs early and clearly
- provide clear error messages
- show users how to fix the issue
- allow easy recovery without losing progress

Errors should be easy to understand and fix.

## Implementation rules

- validate inputs in real time where possible
- use clear, specific error messages
- highlight exactly where the error occurred
- preserve user input when errors happen
- provide clear recovery steps
- avoid blocking progress unnecessarily

## Example

Bad:
- generic error message
- user must restart process
- no indication of what went wrong

Good:
- clear error message with guidance
- input preserved
- user can fix and continue easily

## Fail conditions

- user cannot fix the error
- unclear error messages
- lost input or progress
- user abandons due to frustration

## Enforcement rule

If an error stops progress or causes confusion, redesign until the user can immediately understand and recover.
