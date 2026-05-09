# Design Tokens

## What
Design Tokens are named values for colour, spacing, typography, radius, shadow, motion, and other design decisions.

Tokens make design decisions reusable and consistent.

## Why it matters
Without tokens, interfaces drift into one-off styling.

Good tokens:
- improve consistency
- speed implementation
- support themes
- reduce maintenance
- protect brand and accessibility

Tokens turn visual rules into enforceable system values.

## When to apply
- design systems
- multi-page apps
- themes
- component libraries
- redesigns
- responsive systems
- dark mode

## How to apply

- define semantic tokens for roles
- avoid hard-coded one-off values
- connect tokens to component states
- keep token names meaningful
- preserve accessibility in token choices
- update components through tokens where possible

Tokens should represent intent, not just raw values.

## Implementation rules

- primary action colour must use a semantic token
- spacing must map to a scale
- typography must use named styles or variables
- state colours must be consistent
- tokens must not multiply without purpose
- one-off styling must be justified

## Example

Bad:
- random hex values across components
- several similar spacing values
- dark mode overrides every component manually

Good:
- semantic colour tokens
- spacing scale
- component state tokens
- theme values applied consistently

## Fail conditions

- similar components use different values
- token names describe colour, not role, where role matters
- hard-coded values break consistency
- themes require component-by-component fixes
- tokens create complexity without reuse

## Enforcement rule

If a visual decision repeats, turn it into a clear token or use an existing one.
