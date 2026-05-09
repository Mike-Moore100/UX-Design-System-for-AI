# Doherty Threshold

## What
The Doherty Threshold states that users remain fully engaged when system response time is under ~400 milliseconds.

Interactions that respond within this window feel immediate and continuous.

## Why it matters
Delays break user flow, increase frustration, and reduce trust.

When feedback is slow or missing, users:
- think the system is broken
- repeat actions (double clicks)
- lose confidence and disengage

Fast, visible feedback maintains momentum and keeps users in control.

## When to apply
- all user interactions (clicks, taps, inputs)
- loading states and transitions
- form submissions
- navigation between screens
- any action where the system processes or responds

## How to apply

- provide immediate visual feedback on every interaction
- show loading states instantly if processing takes time
- avoid silent delays or dead states
- ensure transitions feel fast and responsive
- maintain continuous feedback until completion

Users should always know that the system is responding.

## Implementation rules

- initial feedback must occur within 100–200ms
- perceived response must always occur within 400ms
- show loading indicators immediately if delay >200ms
- avoid blocking the interface without feedback
- ensure transitions complete within 200–300ms
- prevent repeated actions by acknowledging input instantly

## Example

Bad:
- click → no response for 1–2 seconds
- no loading indicator
- user clicks again thinking it didn’t work

Good:
- click → immediate visual feedback (button state change)
- loading indicator appears instantly
- clear transition or confirmation when complete

## Fail conditions

- user clicks multiple times
- user waits without feedback
- user assumes the system is broken
- interactions feel slow or unresponsive

## Enforcement rule

Every user action must produce immediate feedback - if there is no visible response, the interaction has failed.
