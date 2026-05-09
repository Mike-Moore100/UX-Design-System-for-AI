# Reduced Motion

## What
Reduced Motion respects users who experience discomfort, distraction, or vestibular symptoms from animation.

Motion must never be required to understand the interface.

## Why it matters
Some motion can cause nausea, dizziness, headaches, or cognitive disruption.

Respecting reduced motion:
- protects user comfort
- supports accessibility settings
- improves focus
- prevents unnecessary distraction
- keeps meaning available without animation

Motion is optional; meaning is not.

## When to apply
- transitions
- parallax
- loading animations
- hover effects
- carousels
- success states
- page changes

## How to apply

- respect prefers-reduced-motion
- replace large motion with subtle fades or instant changes
- avoid parallax and auto-moving content
- keep feedback visible without motion
- pause or stop looping animation
- ensure animation is not the only state signal

The interface should remain clear with motion reduced.

## Implementation rules

- reduced motion preference must be honoured
- essential state changes need non-motion cues
- auto-playing motion must be avoidable
- large directional movement should be reduced
- loading indicators should not rely on intense motion
- animation must not block task completion

## Example

Bad:
- full-screen page slide despite reduced motion
- looping decorative animation near a form
- success only shown through animation

Good:
- instant route transition
- static success confirmation
- subtle opacity change
- paused decorative motion

## Fail conditions

- motion ignores user preference
- animation causes distraction or discomfort
- state meaning disappears without motion
- auto-motion cannot be stopped
- motion delays interaction

## Enforcement rule

If motion is not essential, reduce or remove it for users who request reduced motion.
