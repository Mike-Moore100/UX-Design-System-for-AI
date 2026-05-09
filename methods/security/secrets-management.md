# Secrets Management

## What
Secrets Management protects API keys, tokens, passwords, private keys, and credentials throughout their lifecycle.

Secrets must be treated as toxic data.

## Why it matters
Leaked secrets can expose accounts, infrastructure, and customer data.

Good secrets management:
- prevents accidental exposure
- limits credential blast radius
- supports rotation
- improves operational safety
- reduces incident impact

Secrets should never appear in places they do not belong.

## When to apply
- API keys
- integrations
- environment variables
- logs
- admin tools
- webhooks
- deployment config

## How to apply

- store secrets in secure secret storage
- show secrets only once when necessary
- redact secrets in logs and UI
- scope and rotate keys
- avoid committing secrets
- provide revocation controls

Users and systems should see only what they need.

## Implementation rules

- secrets must not be committed to the repo
- secrets must not be logged
- keys should be scoped and named
- users need revoke and rotate paths
- full secret values should not be repeatedly displayed
- secret inputs must avoid accidental exposure

## Example

Bad:
- API key visible forever in dashboard
- token printed in error log
- full-access key created by default

Good:
- secret shown once
- redacted key display
- scoped token creation
- revoke and rotate controls

## Fail conditions

- secret appears in logs or UI unnecessarily
- key cannot be revoked
- secrets are unscoped
- credentials are stored in code
- rotation path is missing

## Enforcement rule

If a value grants access, store, display, log, and rotate it as a secret.
