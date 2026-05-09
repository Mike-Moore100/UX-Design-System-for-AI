# Audit Logging

## What
Audit Logging records important security, permission, data, and account events for review and investigation.

High-risk actions need a trail.

## Why it matters
Without logs, teams cannot understand what happened after mistakes, abuse, or incidents.

Good audit logging:
- supports accountability
- helps incident response
- improves admin trust
- reveals suspicious patterns
- protects sensitive workflows

Logs should record meaningful events, not private content unnecessarily.

## When to apply
- permission changes
- admin actions
- exports
- billing changes
- auth events
- API key changes
- destructive actions

## How to apply

- log who did what and when
- log affected objects
- log important context without secrets
- make admin-relevant logs reviewable
- protect log integrity
- define retention deliberately

The log should answer what changed and who changed it.

## Implementation rules

- sensitive actions must create audit events
- logs must not store passwords, tokens, or secrets
- timestamps and actor IDs must be recorded
- failed high-risk attempts should be logged
- log access must be permissioned
- audit records should be tamper-resistant where needed

## Example

Bad:
- admin deletes user with no record
- API key shown in logs
- permission changes cannot be reviewed

Good:
- "Maya changed Sam from Member to Admin"
- export event includes actor and time
- failed login burst is logged
- secrets are redacted

## Fail conditions

- sensitive action leaves no trace
- logs contain secrets
- actor or object is missing
- audit trail can be edited casually
- logs are inaccessible to authorised reviewers

## Enforcement rule

If an action changes access, data, billing, or security state, log it safely.
