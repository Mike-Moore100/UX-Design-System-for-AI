# Contrast and Emphasis

## What
Contrast and Emphasis control what stands out, what recedes, and how quickly the user can understand priority.

Emphasis must be earned.

## Why it matters
If too many things are emphasized, nothing is clear.

Good contrast:
- improves readability
- reveals hierarchy
- directs action
- supports accessibility
- reduces scanning effort

## When to apply
- calls to action
- headings
- forms
- navigation
- alerts and states
- dense screens with many competing elements

## How to apply

- emphasize the primary action most
- use lower contrast for supporting content
- use size, weight, spacing, and colour together
- avoid relying on colour alone
- reduce emphasis before adding more emphasis
- check accessibility contrast for text and controls

The screen should have a clear foreground, middle ground, and background.

## Implementation rules

- primary action must have the strongest useful emphasis
- secondary actions must be visibly secondary
- disabled states must be clearly inactive but still readable when text is present
- warnings and errors must stand out without overwhelming the whole screen
- text contrast must meet accessibility requirements
- do not use high contrast on decorative elements

## Example

Bad:
- every button has the same visual weight
- decorative elements are more prominent than actions
- muted text is too low contrast to read
- error states are visually weak

Good:
- one dominant action
- readable supporting text
- clear but controlled state emphasis
- decorative elements stay quiet

## Fail conditions

- everything competes for attention
- primary action is not visually dominant
- text is hard to read
- emphasis is used for decoration
- secondary actions look primary

## Enforcement rule

If emphasis does not match user priority, reduce competing contrast until the intended action is obvious.
