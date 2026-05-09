# Data Visualisation

## What
Data Visualisation turns data into charts, tables, and summaries that help users understand patterns and make decisions.

A chart must clarify the data.

## Why it matters
Poor visualisation can mislead users or hide important information.

Good data visualisation:
- reveals patterns
- supports comparison
- reduces interpretation effort
- improves decision-making
- builds analytical trust

The visual form must match the question.

## When to apply
- dashboards
- reports
- analytics
- finance screens
- admin tools
- product metrics
- comparison views

## How to apply

- choose chart type based on the question
- label axes and units clearly
- avoid unnecessary decoration
- use colour to encode meaning
- show baselines or comparisons where useful
- provide tables or details for exact values

Users should understand what the data means and what to do with it.

## Implementation rules

- chart type must match data relationship
- axes must not mislead
- colour must be accessible and meaningful
- labels must explain units
- legends must be close or unnecessary
- empty and loading data states must be handled

## Example

Bad:
- pie chart with too many slices
- truncated axis exaggerates change
- colour used without labels

Good:
- line chart for trends
- bar chart for comparisons
- labelled units and clear baseline
- accessible colour palette

## Fail conditions

- chart hides the main insight
- visual form misrepresents data
- labels or units are missing
- colour meaning is unclear
- user cannot act on the chart

## Enforcement rule

If a visualisation does not make the data easier to understand, redesign the chart or use a table.
