# Secure Defaults

## What
Secure Defaults means the default configuration should be the safest reasonable option.

Users should not need expert knowledge to avoid insecure settings.

## Why it matters
Most users keep defaults.

Unsafe defaults lead to:
- accidental exposure
- weak account protection
- public data leaks
- preventable abuse
- lower trust

Good defaults protect users before they understand the risk.

## When to apply
- account creation
- privacy settings
- sharing permissions
- API keys
- integrations
- workspace and project settings

## How to apply

- make private safer than public by default
- require deliberate action for risky exposure
- use strong authentication defaults
- limit tokens, exports, and access scopes
- explain high-risk settings in plain language
- make safer choices easy to keep

The safe path should also be the easy path.

## Implementation rules

- new resources should not be public unless the product purpose requires it
- secret keys must never be visible after creation unless necessary
- risky settings must require explicit confirmation
- default session and token lifetimes must be reasonable
- destructive or public-sharing defaults must be conservative
- security settings must be understandable to non-experts

## Example

Bad:
- new projects are public by default
- API keys have full account access
- security warnings are hidden in advanced settings

Good:
- new projects start private
- API keys require scoped access
- risky sharing needs confirmation
- security state is visible in context

## Fail conditions

- default settings expose data
- user must opt into basic protection
- risky actions are hidden behind vague labels
- secrets or tokens are overpowered by default
- security depends on users reading documentation

## Enforcement rule

If the default state is not the safest reasonable state, change the default before adding more explanation.
