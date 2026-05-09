# AI Search Visibility

## What
AI Search Visibility makes public content easier for AI answer engines and AI search systems to discover, understand, cite, and summarize accurately.

It improves eligibility and clarity for AI answers. It does not guarantee inclusion.

## Why it matters
Users increasingly discover products, content, and recommendations through AI-generated answers.

Strong AI search visibility:
- keeps important content crawlable
- makes answers easier to extract
- reduces ambiguity
- supports citation and attribution
- improves trust through evidence and freshness
- helps content appear in search-backed AI experiences

AI systems are more likely to cite content that is clear, specific, current, and easy to parse.

## When to apply
- public landing pages
- product pages
- comparison pages
- documentation
- knowledge bases
- blog posts
- ecommerce pages
- local business pages
- category pages

## How to apply

- make the page indexable and crawlable
- ensure important content exists as visible HTML text
- use clear titles, descriptions, H1s, H2s, and H3s
- answer important questions in concise, self-contained sections
- use tables, lists, definitions, and Q&A blocks where they improve clarity
- support claims with evidence, dates, examples, sources, or product proof
- keep entity names, product names, pricing, locations, and capabilities consistent
- make structured data match the visible page content
- keep content fresh when facts, products, prices, or policies change
- avoid hiding important answers only inside images, PDFs, tabs, or scripts

The page should be easy for a model to quote, summarize, and cite without guessing.

## Implementation rules

- page must be eligible for normal search indexing when AI visibility is desired
- robots.txt must not block search crawlers or AI search crawlers the site wants visibility in
- if ChatGPT search visibility is desired, do not block `OAI-SearchBot`
- blocking model-training crawlers must be handled separately from blocking search or user-triggered retrieval crawlers
- important answers must be available in crawlable HTML, not only in images, PDFs, canvas, or client-only state
- titles, descriptions, headings, and intro copy must align around the same page purpose
- content chunks must be understandable out of context when quoted
- structured data must be valid and consistent with visible content
- `llms.txt` may be added as an experimental content map, but it must not replace sitemap, robots, structured data, internal links, or clear HTML content
- do not add AI-specific claims, files, or schema that are misleading or unsupported

## Example

Bad:
- product page blocks AI search crawlers by accident
- vague headings like "Learn more" and "Powerful features"
- important pricing or capability details only appear in an image
- content makes broad claims without evidence
- stale product information remains on public pages
- `llms.txt` exists but the actual page is thin, unclear, or uncrawlable

Good:
- public page is indexable and crawlable
- H1, title, and description clearly describe the page purpose
- sections answer specific user questions
- comparison tables and FAQs are written in visible HTML
- claims are supported with proof, dates, examples, or sources
- structured data reflects the visible content
- crawler controls separate AI search visibility from model-training preferences

## Fail conditions

- page is not eligible for normal indexing
- desired AI search crawlers are blocked unintentionally
- important answers are hidden from crawlers
- content is too vague for accurate citation
- headings do not describe the sections
- facts are stale or unsupported
- AI-specific files are used as a substitute for useful content

## Enforcement rule

If a page should appear in AI answers, make it crawlable, specific, structured, evidence-backed, and quote-ready before adding experimental AI search files.

