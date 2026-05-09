# Secure Error Handling

## What
Secure Error Handling communicates failure clearly to users without exposing sensitive implementation details.

Errors should help users, not attackers.

## Why it matters
Raw errors can leak stack traces, infrastructure details, account existence, or security logic.

Secure errors:
- guide recovery
- protect system details
- reduce confusion
- support logging
- preserve trust

The user-facing error and internal error are different audiences.

## When to apply
- auth
- payments
- forms
- APIs
- uploads
- admin tools
- integrations

## How to apply

- show useful but safe user messages
- log detailed errors internally
- avoid exposing stack traces
- avoid account enumeration
- provide recovery steps
- use consistent error patterns

Users should know what to do next without seeing internals.

## Implementation rules

- production errors must not expose stack traces
- auth errors must avoid revealing account existence
- internal details must go to logs, not UI
- error IDs can support support requests
- user messages must be actionable
- sensitive values must be redacted

## Example

Bad:
- database exception displayed to user
- "No account exists for this email"
- API key included in error detail

Good:
- "We could not save changes. Try again."
- neutral password reset response
- internal log with error ID
- redacted sensitive values

## Fail conditions

- error leaks implementation detail
- error reveals account existence unnecessarily
- user gets no recovery path
- sensitive values appear in logs or UI
- raw exception reaches production UI

## Enforcement rule

If an error helps an attacker more than a user, rewrite the user message and log details securely.
