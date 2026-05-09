# Cross Browser QA

## What
Cross Browser QA checks that critical flows work across the browsers, engines, and platform constraints the product supports.

Browser compatibility should be risk-based and focused on user impact.

## Why it matters
CSS, JavaScript, forms, media, and platform APIs do not always behave the same everywhere.

Cross-browser QA:
- catches compatibility issues
- protects revenue and activation flows
- improves accessibility reliability
- prevents platform-specific breakage
- reduces support burden

One unsupported API can break an entire flow.

## When to apply
- checkout
- signup
- dashboards
- complex CSS layouts
- file uploads
- media features
- authentication
- mobile web

## How to apply

- define supported browsers and versions
- test critical journeys in each supported engine
- check form controls and validation behaviour
- verify CSS features with fallbacks
- test permissions, uploads, clipboard, camera, and storage when used
- document known limitations

The product should fail gracefully when a platform feature is unavailable.

## Implementation rules

- critical flows must work in supported browsers
- modern APIs must have fallback or clear unsupported states
- CSS features must not break layout without support
- authentication and payment flows need highest priority
- mobile browser behaviour must be checked separately when relevant
- known unsupported environments must be documented

## Example

Bad:
- uses browser-only API without fallback
- layout relies on unsupported CSS
- file upload works in one browser only
- auth popup blocked without recovery

Good:
- support matrix defined
- critical flow checked in major engines
- fallback state for unsupported feature
- documented limitation with alternate path

## Fail conditions

- supported browser cannot complete primary task
- missing API creates silent failure
- browser differences cause layout breakage
- fallback is absent
- compatibility risk is unknown for a critical flow

## Enforcement rule

If a critical journey depends on browser behaviour, verify it in supported engines or provide a fallback.

