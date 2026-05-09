# Perceived Performance

## What
Perceived Performance is how fast a system feels to the user, regardless of actual load time.

Users judge speed based on feedback and responsiveness, not raw performance metrics.

## Why it matters
Users react to perceived delays, not technical ones.

If the system feels slow, users:
- lose trust
- repeat actions
- abandon the task

Fast-feeling systems increase engagement and completion.

## When to apply
- loading states
- navigation between screens
- data fetching and rendering
- any delayed response or processing

## How to apply

- provide immediate visual feedback on all interactions
- use skeleton loaders instead of blank screens
- progressively load content where possible
- prioritise visible content first
- avoid blocking the interface without feedback

The system should always feel active and responsive.

## Implementation rules

- initial feedback within 100–200ms
- show loading states immediately if delay >200ms
- use skeleton loaders instead of spinners where possible
- avoid blank or empty states during loading
- prioritise above-the-fold content
- prevent user uncertainty during delays

## Example

Bad:
- blank screen while loading
- delayed or no feedback

Good:
- skeleton UI appears instantly
- visible loading state
- progressive content rendering

## Fail conditions

- user thinks system is slow
- user clicks multiple times
- user unsure if anything is happening

## Enforcement rule

If the system appears idle or unresponsive, add immediate feedback until it feels fast and continuous.
