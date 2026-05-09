# Rate Limiting

## What
Rate Limiting controls how often users, IPs, tokens, or systems can perform actions.

Abuse grows when high-cost actions are unlimited.

## Why it matters
Unlimited actions enable brute force, spam, scraping, resource exhaustion, and denial of service.

Good rate limiting:
- reduces abuse
- protects availability
- slows attacks
- controls cost
- improves product reliability

Limits should protect legitimate users and block abusive patterns.

## When to apply
- login attempts
- password resets
- signup
- invites
- search
- AI generation
- uploads
- API endpoints

## How to apply

- limit high-risk actions by actor and context
- use progressive throttling where useful
- give helpful but safe error messages
- avoid revealing sensitive account information
- log suspicious activity
- provide recovery for legitimate users

The system should slow abuse before it harms users or infrastructure.

## Implementation rules

- auth attempts must be rate limited
- costly endpoints need usage protection
- limits must be enforced server-side
- error messages must not leak account existence
- trusted users may need different limits
- rate limit events should be observable

## Example

Bad:
- unlimited password reset emails
- unlimited AI generation requests
- login brute force has no delay

Good:
- throttled login attempts
- capped invite sends
- per-token API limits
- safe message after too many attempts

## Fail conditions

- high-risk action is unlimited
- limit can be bypassed client-side
- error exposes sensitive information
- legitimate user has no recovery path
- abuse signals are not logged

## Enforcement rule

If an action can be abused at scale, rate limit it and provide safe recovery for legitimate users.
