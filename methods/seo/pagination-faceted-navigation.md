# Pagination Faceted Navigation

## What
Pagination Faceted Navigation controls how large lists, filters, and sorted views are exposed to users and search engines.

The system must help discovery without creating crawl traps or duplicate pages.

## Why it matters
Faceted interfaces can generate thousands of low-value URLs.

Good handling:
- improves crawl efficiency
- protects important category pages
- reduces duplicate content
- supports user exploration
- prevents index bloat

Search engines should see the valuable paths, not every possible filter combination.

## When to apply
- ecommerce categories
- marketplaces
- directories
- job boards
- documentation lists
- search result pages
- product collections

## How to apply

- decide which filter combinations deserve indexable pages
- keep low-value filtered URLs out of the index
- use clean URLs for valuable categories
- preserve user-selected filters in the interface
- avoid infinite URL combinations
- make pagination crawlable when pages contain valuable items
- provide internal links to important category paths

The experience should support both user refinement and search clarity.

## Implementation rules

- valuable category URLs must be crawlable and internally linked
- low-value filter combinations must not be indexed
- sorting parameters should usually be canonicalised or excluded
- pagination must be usable without breaking navigation
- filters must not create uncontrolled URL sprawl
- canonical and noindex rules must not conflict

## Example

Bad:
- every filter and sort combination is indexable
- pagination only works through client state with no crawlable paths
- category pages canonicalise to unrelated pages
- search pages appear in the sitemap

Good:
- curated indexable category pages
- crawlable pagination where useful
- low-value filters excluded
- internal links to priority collections

## Fail conditions

- crawl budget is wasted on filter combinations
- important pages are hidden
- duplicate URLs compete
- user filters break shareability
- sitemap includes low-value generated URLs

## Enforcement rule

If faceted navigation creates many URLs, define which paths are indexable before releasing the interface.

