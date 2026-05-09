# XSS Prevention

## What
XSS Prevention stops untrusted content from executing script in a user's browser.

User-controlled content must never become executable by accident.

## Why it matters
Cross-site scripting can steal sessions, alter pages, perform actions, and expose user data.

Good XSS prevention:
- protects user sessions
- preserves interface integrity
- secures user-generated content
- reduces account takeover risk
- protects trust

Rendering content is a security boundary.

## When to apply
- comments
- rich text
- markdown
- profile fields
- imported content
- search results
- admin tools

## How to apply

- escape output by default
- sanitise allowed rich content
- avoid dangerously setting HTML
- use content security policy where appropriate
- validate URLs and embeds
- treat admin input as untrusted too

The safest output is encoded output.

## Implementation rules

- untrusted content must be escaped before rendering
- rich text needs a proven sanitizer
- inline event handlers must be avoided
- URL protocols must be allowlisted
- CSP should reduce script execution risk
- admin-only fields are still untrusted

## Example

Bad:
- rendering user HTML directly
- allowing javascript: URLs
- trusting imported markdown

Good:
- escaped output
- sanitized markdown
- allowlisted URL protocols
- restrictive content security policy

## Fail conditions

- untrusted content executes script
- sanitizer is missing or custom and weak
- dangerous HTML is allowed unnecessarily
- URL validation is absent
- admin input bypasses protection

## Enforcement rule

If content comes from outside the trusted codebase, escape or sanitize it before rendering.
