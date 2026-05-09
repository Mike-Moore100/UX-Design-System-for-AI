# Output Trust

## What
Output Trust helps users understand, evaluate, and verify AI-generated content before acting on it.

AI output should be useful without pretending to be certain when it is not.

## Why it matters
AI systems can be fluent and wrong.

Output trust:
- reduces overreliance
- improves decision quality
- supports accountability
- makes uncertainty visible
- helps users verify important claims

Confidence without evidence is dangerous in high-stakes contexts.

## When to apply
- AI answers
- summaries
- recommendations
- generated code
- legal, financial, medical, or security-adjacent content
- research tools
- decision support

## How to apply

- show sources, citations, or evidence when claims need support
- separate generated content from verified facts
- expose uncertainty where it affects decisions
- make important assumptions visible
- provide ways to inspect reasoning artifacts without exposing chain-of-thought
- let users edit, reject, or regenerate output

The user should know what can be trusted, checked, or changed.

## Implementation rules

- high-impact claims must include evidence or verification paths
- uncertainty must be visible when it affects action
- generated output must be distinguishable from user-authored or verified content
- citations must link to real accessible sources when used
- the interface must not imply guaranteed correctness
- users must have a clear way to correct or reject output

## Example

Bad:
- generated answer presented as fact with no source
- confidence badge without meaning
- AI changes production content automatically
- user cannot see or edit assumptions

Good:
- sources and dates shown
- assumptions listed
- generated draft is editable
- high-risk recommendation requires review

## Fail conditions

- output appears more certain than it is
- claims cannot be verified
- user cannot correct the result
- generated content is indistinguishable from approved content
- citations are missing, broken, or decorative

## Enforcement rule

If an AI output could influence a meaningful decision, make its evidence, uncertainty, and user controls visible.

