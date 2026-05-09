# Loading Strategy

## What
Loading Strategy defines how the product reveals progress while data, assets, routes, or AI outputs are still loading.

Waiting should feel informed, stable, and purposeful.

## Why it matters
Users tolerate waiting better when they understand that progress is happening.

Good loading strategy:
- reduces perceived delay
- prevents layout jumps
- protects trust
- keeps users oriented
- improves completion during slow network or model calls

Blank waiting feels broken.

## When to apply
- route transitions
- dashboards
- search results
- AI generation
- checkout
- uploads
- imports
- slow API calls

## How to apply

- show immediate feedback after user action
- reserve space for incoming content
- use skeletons only when layout is predictable
- use progress indicators for long or staged tasks
- explain delays when the wait may be long
- keep previous useful content visible when possible

The user should know the system is working and what will happen next.

## Implementation rules

- every action over a noticeable delay must show feedback
- loading UI must not shift layout when content arrives
- skeletons must resemble final content
- long-running tasks must show status or staged progress
- errors must replace infinite loading states
- loading copy must be specific when time or risk is meaningful

## Example

Bad:
- blank page during route load
- spinner with no context for a 30-second import
- skeleton layout does not match final content
- loading state never resolves on failure

Good:
- instant button feedback
- stable skeleton
- progress messages for import steps
- retryable error if loading fails

## Fail conditions

- user cannot tell if anything is happening
- layout jumps when content arrives
- loading state hides useful existing content
- long wait has no explanation
- failures look like endless loading

## Enforcement rule

If a user must wait, show stable feedback that explains progress and preserves orientation.

