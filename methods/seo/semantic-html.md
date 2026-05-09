# Semantic HTML

## What
Semantic HTML uses meaningful elements to communicate page structure to browsers, assistive technology, and search engines.

Semantic structure helps machines understand human content.

## Why it matters
Search engines and assistive technologies rely on structure to interpret pages.

Good semantic HTML:
- clarifies page hierarchy
- improves crawlability
- supports accessibility
- reduces implementation ambiguity
- strengthens content meaning

Structure should reflect the page's actual information architecture.

## When to apply
- public pages
- blogs and articles
- documentation
- product pages
- navigation
- tables and data content

## How to apply

- use one clear h1
- use headings to represent content hierarchy
- use main, nav, header, footer, section, and article appropriately
- use lists for lists and tables for tabular data
- make links descriptive
- avoid hiding important content from the DOM

The markup should explain the page without styling.

## Implementation rules

- h1 must describe the page topic
- heading order must be logical
- navigation must be crawlable
- important text must not exist only in images
- buttons and links must match their behaviour
- structured content should use appropriate HTML elements

## Example

Bad:
- heading levels chosen only for visual size
- main content rendered as non-semantic divs
- important copy embedded in images
- links labelled "click here"

Good:
- meaningful heading structure
- semantic page regions
- descriptive links
- crawlable text content

## Fail conditions

- crawlers cannot understand page hierarchy
- important content is inaccessible or hidden
- headings are random or duplicated
- links lack meaning
- visual structure and HTML structure conflict

## Enforcement rule

If the page structure only works visually, rebuild it with semantic HTML.
