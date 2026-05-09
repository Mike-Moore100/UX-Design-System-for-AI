# Input Validation

## What
Input Validation ensures all user-controlled data is checked, constrained, and safely handled before it affects the system.

All input is untrusted until validated.

## Why it matters
Unvalidated input is a common source of injection, data corruption, broken workflows, and security vulnerabilities.

Strong validation:
- prevents malformed data
- reduces attack surface
- improves error recovery
- protects downstream systems
- increases user confidence

Validation must happen in the interface and on the server.

## When to apply
- forms
- search
- uploads
- API inputs
- URL parameters
- rich text or markdown
- imported data

## How to apply

- define allowed input, not only blocked input
- validate on the server before trust
- constrain inputs in the UI where useful
- provide clear recovery messages
- sanitize output where content is rendered
- handle files, URLs, and rich text with extra care

Users should be guided toward valid input, but the system must enforce it.

## Implementation rules

- client validation is usability, not security
- server validation is mandatory
- error messages must not leak sensitive implementation detail
- file uploads must check type, size, and handling path
- rendered user content must be escaped or sanitized
- validation rules must match actual business rules

## Example

Bad:
- only front-end validation
- accepting arbitrary file uploads
- rendering user HTML directly
- generic "Something went wrong" errors

Good:
- client hints plus server enforcement
- allowlisted input formats
- escaped or sanitized output
- clear validation messages

## Fail conditions

- user input reaches storage or execution without validation
- validation rules differ between client and server
- dangerous content can be rendered
- errors leak stack traces or system details
- upload handling is unrestricted

## Enforcement rule

If input can cross a trust boundary, validate it server-side and handle it safely before use.
