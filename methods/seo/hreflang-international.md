# Hreflang International

## What
Hreflang International helps search engines serve the correct language or regional version of equivalent pages.

International SEO must match real localisation, not only translated keywords.

## Why it matters
Users need the right language, currency, region, and legal context.

Good hreflang implementation:
- reduces wrong-region results
- consolidates equivalent page relationships
- improves international relevance
- supports regional conversion
- prevents duplicate language confusion

Incorrect hreflang can create search routing problems.

## When to apply
- multilingual sites
- regional product pages
- country-specific pricing
- international documentation
- global ecommerce
- language-specific landing pages

## How to apply

- create equivalent pages for each language or region
- use correct language and region codes
- include reciprocal hreflang references
- provide an x-default when useful
- keep canonical tags language-specific
- localise currency, legal details, examples, and support paths where relevant

The user should land on the version built for their language or region.

## Implementation rules

- hreflang URLs must return valid pages
- hreflang sets must be reciprocal
- language and region codes must be valid
- canonical tags must not point all regions to one language version
- translated pages must be substantially equivalent
- localised content must match user expectations

## Example

Bad:
- all language versions canonicalise to English
- hreflang references missing reciprocal tags
- translated page keeps wrong currency and support details
- region codes are invalid

Good:
- correct language-region mapping
- reciprocal hreflang set
- x-default selector page
- localised pricing and legal copy where needed

## Fail conditions

- wrong language appears in search
- hreflang tags conflict with canonicals
- equivalent pages are missing
- regional content is not actually localised
- invalid codes or broken URLs are used

## Enforcement rule

If multiple language or region versions exist, implement valid reciprocal hreflang and localisation before scaling international pages.

