# Dependency Safety

## What
Dependency Safety manages third-party packages, scripts, SDKs, and services so they do not introduce avoidable risk.

Every dependency is part of the attack surface.

## Why it matters
Dependencies can ship vulnerabilities, tracking, instability, or supply-chain risk.

Good dependency safety:
- reduces attack surface
- improves reliability
- protects user data
- controls bundle size
- supports maintainability

Use dependencies deliberately, not casually.

## When to apply
- npm packages
- analytics scripts
- payment SDKs
- auth libraries
- UI libraries
- embeds
- build tools

## How to apply

- prefer proven maintained libraries
- avoid packages for trivial tasks
- review permissions and data access
- keep dependencies updated
- remove unused dependencies
- monitor vulnerabilities

The dependency must earn its cost and risk.

## Implementation rules

- dependencies must have a clear purpose
- unmaintained packages should be avoided
- security updates must be applied promptly
- third-party scripts must be justified
- unused packages must be removed
- sensitive data shared with third parties must be deliberate

## Example

Bad:
- package added for one small helper
- abandoned auth library
- multiple analytics scripts with unknown data access

Good:
- maintained security library
- lockfile committed
- dependency audit reviewed
- unused packages removed

## Fail conditions

- dependency is unmaintained
- package adds unnecessary risk
- third-party script collects unclear data
- vulnerabilities are ignored
- dependency exists without product need

## Enforcement rule

If a dependency adds risk without clear value, remove it or replace it with a safer option.
