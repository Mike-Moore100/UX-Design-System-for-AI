# Auth and Session Safety

## What
Auth and Session Safety protects account access, authentication flows, sessions, and recovery paths.

Authentication must be secure and understandable.

## Why it matters
Account systems are high-risk because they control identity, data, billing, and permissions.

Safe auth:
- prevents account takeover
- protects session integrity
- supports secure recovery
- reduces user confusion
- builds trust in sensitive moments

Auth flows must be both secure and usable.

## When to apply
- login
- signup
- password reset
- magic links
- multi-factor authentication
- session timeout
- account recovery

## How to apply

- use proven authentication patterns
- protect reset and invitation flows
- avoid leaking whether an account exists
- make session state visible when useful
- require re-authentication for high-risk actions
- provide clear recovery without exposing accounts

Users should know what is happening without attackers learning too much.

## Implementation rules

- password reset responses must avoid account enumeration
- sessions must be invalidated on logout
- high-risk changes should require fresh authentication
- MFA setup and recovery must be clear
- auth tokens and magic links must expire
- authentication errors must be helpful but not revealing

## Example

Bad:
- "No account exists for this email"
- reset links never expire
- changing email does not require re-authentication
- logout only changes local UI state

Good:
- neutral reset confirmation
- expiring recovery links
- fresh auth before sensitive changes
- server-side session invalidation

## Fail conditions

- auth flow leaks account existence
- session remains valid after logout
- recovery links are long-lived
- sensitive changes need no re-authentication
- MFA recovery is unclear or unsafe

## Enforcement rule

If an auth flow protects identity or access, use proven secure patterns and avoid revealing unnecessary information.
