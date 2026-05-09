# Structured Data

## What
Structured Data adds machine-readable schema that helps search engines understand page entities, content type, and eligible rich results.

Schema should describe what is truly visible and useful on the page.

## Why it matters
Search engines rely on clear signals to interpret content.

Good structured data:
- improves page understanding
- supports rich result eligibility
- clarifies entities and relationships
- reduces ambiguity
- strengthens content quality signals

Invalid or misleading schema can harm trust.

## When to apply
- articles
- product pages
- local business pages
- FAQs
- how-to content
- reviews
- events
- software product pages

## How to apply

- choose schema types that match the visible content
- include required and recommended properties
- keep schema consistent with on-page copy
- validate JSON-LD before release
- update schema when content changes
- avoid marking up hidden or misleading information

The structured data should describe the page, not exaggerate it.

## Implementation rules

- schema type must match the page purpose
- required properties must be complete
- structured data must reflect visible content
- ratings, prices, availability, and dates must be accurate
- JSON-LD must be valid
- do not add schema solely to chase unsupported rich results

## Example

Bad:
- FAQ schema for questions not visible on the page
- fake review ratings
- product schema missing price or availability
- article dates that do not match the page

Good:
- accurate product schema
- article schema with author and dates
- FAQ schema for visible FAQs
- validated JSON-LD

## Fail conditions

- schema contradicts visible content
- required fields are missing
- generated markup is invalid
- rich result eligibility is pursued dishonestly
- structured data is stale

## Enforcement rule

If structured data cannot be made accurate and valid, omit it rather than publishing misleading markup.

