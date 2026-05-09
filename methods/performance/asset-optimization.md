# Asset Optimization

## What
Asset Optimization reduces unnecessary cost from images, video, fonts, icons, scripts, and third-party resources.

Assets should earn their weight.

## Why it matters
Heavy assets slow pages, increase data cost, and make products feel less professional.

Optimised assets:
- improve loading speed
- reduce bandwidth
- protect mobile users
- improve Core Web Vitals
- keep visual quality purposeful

Beautiful assets that slow the primary task are not product quality.

## When to apply
- marketing pages
- media-heavy screens
- product screenshots
- dashboards
- icon systems
- custom fonts
- embedded videos
- third-party scripts

## How to apply

- compress and resize images for their rendered size
- use modern image formats where supported
- lazy-load below-the-fold media
- preload only critical assets
- limit font weights and variants
- remove unused icons, scripts, and embeds
- replace heavy assets when lighter UI conveys the same meaning

The product should look sharp without making the user wait unnecessarily.

## Implementation rules

- images must not be much larger than display requirements
- below-the-fold media should be lazy-loaded
- critical visual assets must have stable dimensions
- fonts must be limited to needed weights/styles
- third-party scripts must justify their performance and privacy cost
- decorative assets must not block primary content

## Example

Bad:
- 4 MB hero image for a small card
- loads six font weights
- embeds video before primary content
- third-party script blocks rendering

Good:
- responsive image sizes
- compressed visual assets
- minimal font set
- deferred embeds
- only critical assets preloaded

## Fail conditions

- decorative assets delay useful content
- image size is disproportionate
- font loading causes visible instability
- third-party scripts slow the page
- unused assets remain in the critical path

## Enforcement rule

If an asset does not improve user understanding or trust enough to justify its cost, optimise it or remove it.

