# Interaction Responsiveness

## What
Interaction Responsiveness ensures clicks, taps, typing, dragging, scrolling, and navigation respond quickly enough to feel under the user's control.

Responsiveness is the user's felt speed.

## Why it matters
Slow interactions damage trust even when initial load is fast.

Responsive interaction:
- improves perceived quality
- reduces repeated clicks
- prevents input errors
- supports accessibility
- makes complex tools feel professional

Users blame themselves when the interface lags.

## When to apply
- forms
- editors
- dashboards
- navigation
- filters
- search
- drag and drop
- AI prompt inputs

## How to apply

- avoid blocking the main thread during input
- debounce expensive filtering or search work
- provide optimistic feedback where safe
- keep transitions short and purposeful
- split heavy rendering into smaller work
- prevent duplicate submissions during pending actions

The interface should acknowledge intent immediately.

## Implementation rules

- buttons and controls must show pressed, pending, or disabled states quickly
- typing must not lag behind the user's input
- expensive updates must be deferred, debounced, memoised, or virtualised
- repeated actions must not create duplicate side effects
- animations must not block interaction
- responsiveness must be checked on realistic devices where possible

## Example

Bad:
- search input freezes while filtering a large table
- submit button does nothing for two seconds
- user can click checkout twice
- drag interaction drops frames badly

Good:
- immediate pending state
- debounced search
- virtualised table rows
- duplicate submission protection
- interaction remains smooth during updates

## Fail conditions

- input visibly lags
- users repeat clicks because feedback is missing
- heavy rendering blocks controls
- animations reduce responsiveness
- slow action creates duplicate requests

## Enforcement rule

If the user performs an action, the interface must acknowledge it immediately and prevent unsafe repeated input.

