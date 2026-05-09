# Recognition Over Recall

## What
Recognition Over Recall means users should be able to recognise options, actions, and states instead of remembering information from elsewhere.

Interfaces should make the right choice visible.

## Why it matters
Memory is limited and context fades quickly.

Recognition:
- reduces cognitive load
- speeds up decisions
- lowers error rates
- improves confidence
- helps new users succeed faster

Users should not have to remember hidden rules to use the product.

## When to apply
- navigation
- forms
- settings
- command menus
- onboarding
- dashboards
- multi-step flows

## How to apply

- show available options in context
- use familiar labels and visible states
- keep important information close to the decision
- provide previews, examples, and defaults
- avoid making users remember values from previous screens
- make recently used or likely choices easy to find

The interface should carry the memory burden.

## Implementation rules

- labels must be visible where decisions are made
- selected states must remain visible
- important constraints must appear near the control
- previous choices must be summarised in later steps
- examples should clarify unfamiliar inputs
- avoid hidden commands for primary actions

## Example

Bad:
- user must remember pricing limits from another page
- selected filters disappear after applying
- form constraints only appear after error

Good:
- selected filters stay visible
- plan limits appear near upgrade choice
- examples appear inside complex inputs
- previous step summary is visible before confirmation

## Fail conditions

- user must remember information from another screen
- selected state is unclear
- constraints are hidden until failure
- labels rely on internal terminology
- primary choices are not visible

## Enforcement rule

If the user must recall important information to proceed, make that information visible at the decision point.
