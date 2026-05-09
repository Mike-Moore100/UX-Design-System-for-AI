# Feedback Loops

## What
Feedback Loops are the system responses that inform users what is happening after they take an action.

Every action must produce a clear, immediate, and understandable reaction.

## Why it matters
Without feedback, users feel lost, unsure, and out of control.

Lack of feedback leads to:
- repeated actions (double clicks)
- confusion about system state
- reduced trust and confidence

Clear feedback creates:
- certainty
- control
- smooth interaction flow

## When to apply
- button clicks and interactions
- form submissions
- navigation and state changes
- loading and processing states
- success and error outcomes

## How to apply

- provide immediate visual response on interaction
- show system state changes clearly
- confirm success actions explicitly
- communicate errors with clear recovery paths
- maintain feedback throughout the entire interaction lifecycle

Feedback should be continuous until the action is complete.

## Implementation rules

- every interaction must trigger visible feedback within 100–200ms
- loading states must appear immediately if processing is required
- success states must confirm completion clearly
- error states must explain the issue and how to fix it
- do not allow silent failures or invisible state changes
- ensure feedback is consistent across all components

## Example

Bad:
- click → no visible response
- action completes silently
- user unsure if anything happened

Good:
- click → immediate visual change (button state, animation)
- loading indicator appears if needed
- clear success confirmation or next step shown

## Fail conditions

- user repeats actions unnecessarily
- user unsure if action worked
- no visible system response
- inconsistent feedback across interactions

## Enforcement rule

If an action does not produce clear, immediate feedback, it has failed - every interaction must visibly respond and confirm state.
