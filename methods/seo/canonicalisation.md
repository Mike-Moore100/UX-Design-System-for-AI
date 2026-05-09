# Canonicalisation

## What
Canonicalisation tells search engines which URL should be treated as the preferred version when duplicate or similar pages exist.

Canonical signals should match the site's real content strategy.

## Why it matters
Duplicate URLs split ranking signals and create indexing confusion.

Strong canonicalisation:
- consolidates authority
- prevents duplicate content problems
- improves crawl efficiency
- clarifies preferred URLs
- protects search performance during filtering or tracking

Search engines should not have to guess which page matters.

## When to apply
- product variants
- filtered category pages
- tracking parameters
- syndicated content
- pagination
- duplicate landing pages
- http to https migrations

## How to apply

- choose the URL that should rank
- add self-referencing canonicals on canonical pages
- point duplicate or parameterised URLs to the preferred version
- keep internal links aligned with canonical URLs
- avoid canonical chains
- use redirects when duplicates should not be accessible

The canonical URL should be the version users and search engines are meant to trust.

## Implementation rules

- every indexable page should have a clear canonical signal
- canonical targets must return a valid 200 response
- canonical targets must contain substantially equivalent content
- internal links should use canonical URLs
- canonical tags must not conflict with redirects or noindex
- avoid canonicalising unrelated pages

## Example

Bad:
- filtered URLs all indexable with no canonical
- canonical points to a 404
- canonical target has different content
- internal links use tracking URLs

Good:
- clean canonical URL
- self-referencing canonical on primary page
- duplicate variants point to the right source
- internal links match preferred URLs

## Fail conditions

- search engines receive conflicting signals
- duplicate pages compete
- canonical target is unavailable
- canonical points to unrelated content
- important variant pages are accidentally suppressed

## Enforcement rule

If similar URLs exist, define the preferred URL and align canonical tags, links, redirects, and indexing rules around it.

