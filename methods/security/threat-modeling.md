# Threat Modeling

## What
Threat Modeling identifies what can go wrong, who could cause it, and how the system should prevent or reduce harm.

Security starts by understanding risk.

## Why it matters
Without threat modeling, teams protect obvious areas while missing real attack paths.

Threat modeling:
- reveals trust boundaries
- prioritises risks
- improves design decisions
- reduces costly fixes later
- supports safer defaults

Risk should be considered before implementation hardens around it.

## When to apply
- auth flows
- payments
- admin tools
- data exports
- uploads
- integrations
- permission changes

## How to apply

- identify assets and sensitive actions
- identify actors and misuse cases
- map trust boundaries
- list likely threats
- design mitigations
- verify mitigations in UI and code

The product should make high-risk paths visible before they become incidents.

## Implementation rules

- sensitive data must be identified
- trust boundaries must be explicit
- high-risk actions need mitigation
- assumptions must be documented
- client-side controls must not replace server checks
- security risks must influence UX, not only backend logic

## Example

Bad:
- admin export flow built with no permission review
- upload feature has no abuse analysis
- billing changes treated like normal settings

Good:
- mapped actors, assets, and threats
- permission checks at boundaries
- confirmation for sensitive actions
- logging for high-risk changes

## Fail conditions

- sensitive action has no risk review
- trust boundary is unclear
- mitigation is missing or only visual
- likely misuse case is ignored
- risk is discovered only after implementation

## Enforcement rule

If a feature touches data, identity, money, or permissions, model the threats before treating it as complete.
