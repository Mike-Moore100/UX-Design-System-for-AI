# Robots Indexing

## What
Robots Indexing controls which pages search engines can crawl, index, and show in results.

Indexing rules should protect search quality without hiding valuable pages.

## Why it matters
Search engines need access to the right pages and exclusion from the wrong ones.

Good indexing control:
- improves crawl efficiency
- prevents thin or private pages from ranking
- protects duplicate surfaces
- supports launch readiness
- avoids accidental deindexing

One wrong directive can remove important pages from search.

## When to apply
- public websites
- staging environments
- internal app pages
- search result pages
- filtered pages
- login-protected areas
- duplicate content
- site migrations

## How to apply

- decide which pages should be indexable
- use robots.txt for crawl guidance
- use meta robots or headers for indexing control
- keep private or account pages out of search
- make important assets crawlable when needed for rendering
- test staging and production rules separately

Search engines should crawl and index only the surfaces intended for discovery.

## Implementation rules

- important public pages must not be blocked
- private or low-value pages must not be indexable
- staging must not be indexed
- noindex pages should not be blocked from crawling when the directive must be seen
- robots.txt must not be treated as a privacy control
- sitemap URLs should be indexable canonical pages

## Example

Bad:
- production site ships with noindex
- login pages appear in search
- CSS or JS needed for rendering is blocked
- sitemap contains blocked URLs

Good:
- public pages indexable
- staging protected
- internal app screens excluded
- sitemap contains clean canonical URLs

## Fail conditions

- valuable pages cannot be indexed
- private pages can appear in search
- robots and meta directives conflict
- sitemap sends low-quality URLs
- crawl budget is wasted on irrelevant pages

## Enforcement rule

If a page should or should not appear in search, make that indexing decision explicit and verify the directive path.

