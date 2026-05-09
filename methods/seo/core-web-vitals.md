# Core Web Vitals

## What
Core Web Vitals measure real user experience signals related to loading, responsiveness, and visual stability.

Performance is part of search quality and product quality.

## Why it matters
Slow or unstable pages frustrate users and reduce trust.

Strong performance:
- improves user experience
- supports SEO
- reduces abandonment
- improves perceived quality
- helps mobile users

Speed must be designed and engineered together.

## When to apply
- public pages
- landing pages
- blogs
- product pages
- dashboards with heavy content
- media-heavy screens
- mobile experiences

## How to apply

- optimise largest visible content
- avoid layout shifts
- reduce blocking JavaScript
- use responsive images
- preserve stable dimensions for media
- provide immediate feedback for interactions

The page should load quickly and stay visually stable.

## Implementation rules

- images and media need defined dimensions
- critical content must not be delayed unnecessarily
- third-party scripts must be justified
- layout must not jump during loading
- interaction feedback must feel immediate
- mobile performance must be considered, not assumed

## Example

Bad:
- hero image loads late and shifts layout
- heavy scripts block first render
- buttons lag after tap
- ads or embeds move content

Good:
- optimised media
- stable layout boxes
- deferred non-critical scripts
- immediate interaction feedback

## Fail conditions

- page feels slow before content appears
- layout shifts during load
- user input feels delayed
- media is oversized or unoptimised
- third-party scripts dominate load time

## Enforcement rule

If performance harms loading, responsiveness, or stability, simplify and optimise before adding more content.
