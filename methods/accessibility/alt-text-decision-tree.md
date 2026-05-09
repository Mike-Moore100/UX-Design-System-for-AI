# Alt Text Decision Tree

## What
Alt Text Decision Tree is the practice of deciding whether an image needs descriptive alt text, empty alt text, or adjacent text support.

Not every image needs description, but every image needs a decision.

## Why it matters
Images can communicate meaning, decoration, or function.

Good alt handling:
- preserves meaning
- avoids redundant announcements
- supports screen reader users
- improves content quality
- prevents broken image experiences

Alt text should match the image's purpose.

## When to apply
- product screenshots
- charts
- icons
- illustrations
- avatars
- buttons with images
- marketing visuals

## How to apply

- describe meaningful images
- use empty alt for decorative images
- describe function for image buttons
- summarise charts and data visuals
- avoid repeating nearby text
- keep descriptions concise and useful

The user should receive the same meaning, not a literal pixel inventory.

## Implementation rules

- decorative images must use empty alt
- functional images must describe the action
- informative images must describe the meaning
- complex images need adjacent explanation
- alt text must not start with "image of" unless needed
- missing alt is not acceptable

## Example

Bad:
- alt="image"
- decorative background read aloud
- product chart with no summary

Good:
- alt="" for decorative flourish
- alt="Search"
- chart summary in nearby text
- concise screenshot description

## Fail conditions

- meaningful image has no alternative
- decorative image creates noise
- alt text repeats nearby copy
- chart meaning is unavailable
- image button has no action name

## Enforcement rule

If an image carries meaning or function, provide an equivalent alternative; if it does not, hide it from assistive technology.
