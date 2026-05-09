# Edge Case States

## What
Edge Case States covers unusual but likely conditions such as empty data, large data, slow networks, permissions, errors, and partial access.

Good products handle the weird moments.

## Why it matters
Real users rarely stay on the perfect happy path.

Edge-case coverage:
- prevents dead ends
- protects trust
- improves supportability
- reveals hidden assumptions
- makes products feel complete

AI-built products often look polished until real data appears.

## When to apply
- dashboards
- forms
- settings
- search
- permissions
- data imports
- AI generation
- billing

## How to apply

- list the states the screen can enter
- test empty, loading, error, success, and partial states
- test unusually long and short content
- test missing permissions or expired sessions
- test large data sets and no results
- ensure each state has a recovery path

The interface should guide the user even when conditions are imperfect.

## Implementation rules

- empty state must explain what happened and what to do next
- errors must be recoverable
- long content must not break layout
- partial permissions must be clear
- large lists must remain usable
- expired or unavailable states must not lose user work unnecessarily

## Example

Bad:
- blank dashboard when no data exists
- long customer name breaks card layout
- expired session loses a completed form
- search returns nothing with no recovery

Good:
- empty state with action
- robust text wrapping
- session recovery path
- zero-results guidance
- permission state explains access limits

## Fail conditions

- state becomes blank or confusing
- user has no recovery path
- real data breaks layout
- permissions fail silently
- errors destroy user progress

## Enforcement rule

If a likely state can occur, design and verify the state before calling the screen complete.

