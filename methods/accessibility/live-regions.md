# Live Regions

## What
Live Regions announce dynamic updates to assistive technology when content changes without a page reload.

Dynamic interfaces need accessible feedback.

## Why it matters
Screen reader users may not notice changes that appear visually elsewhere on the page.

Good live regions:
- announce important updates
- confirm actions
- explain loading and errors
- preserve orientation
- reduce uncertainty

Updates should be communicated without interrupting unnecessarily.

## When to apply
- form validation
- search results
- loading states
- notifications
- chat
- autosave
- async actions

## How to apply

- announce important status changes
- use polite announcements for normal updates
- use assertive announcements only for urgent messages
- avoid announcing every minor change
- keep messages concise
- ensure visual and announced messages match

The announcement should help the user continue.

## Implementation rules

- async success and failure states need accessible feedback
- validation summaries should be announced when relevant
- loading completion should be communicated
- urgent errors may use assertive live regions
- repeated announcements must not create noise
- live region text must be meaningful on its own

## Example

Bad:
- search results update with no announcement
- autosave fails silently
- every keystroke triggers a screen reader message

Good:
- "12 results found"
- "Changes saved"
- "Payment failed. Check card details."
- loading status announced politely

## Fail conditions

- dynamic change is invisible to assistive technology
- announcements are too frequent
- urgent errors are missed
- announced text lacks context
- visual and announced messages conflict

## Enforcement rule

If content changes without navigation, announce important updates in a controlled and meaningful way.
