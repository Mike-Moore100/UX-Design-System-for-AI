# CSRF Protection

## What
CSRF Protection prevents a malicious site from causing an authenticated user to perform unwanted actions.

Authenticated actions need request integrity.

## Why it matters
Users can be logged in while visiting hostile pages elsewhere.

CSRF protection:
- prevents unwanted state changes
- protects account settings
- reduces abuse of authenticated sessions
- supports trust in sensitive actions
- hardens form submissions

The system must know the request came from the real interface.

## When to apply
- forms that change state
- account settings
- billing actions
- admin actions
- destructive actions
- cookie-based sessions
- authenticated APIs

## How to apply

- use CSRF tokens for state-changing requests
- use same-site cookies appropriately
- require non-GET methods for state changes
- verify origin or referer where useful
- avoid putting state-changing actions in links
- combine with confirmation for sensitive actions

CSRF protection must be server-enforced.

## Implementation rules

- GET requests must not change state
- state-changing forms need CSRF protection when using cookies
- tokens must be validated server-side
- same-site cookie settings must be deliberate
- sensitive actions need stronger verification
- failed CSRF checks must not leak unnecessary detail

## Example

Bad:
- delete account via GET link
- cookie auth with no CSRF token
- cross-origin form can change settings

Good:
- POST with CSRF token
- SameSite cookies configured
- origin checks for sensitive endpoints
- confirmation for destructive changes

## Fail conditions

- authenticated state changes lack request verification
- GET endpoint mutates data
- token exists but is not validated
- cookie policy is unsafe by default
- sensitive action can be triggered cross-site

## Enforcement rule

If an authenticated request changes state, protect it from cross-site request forgery.
