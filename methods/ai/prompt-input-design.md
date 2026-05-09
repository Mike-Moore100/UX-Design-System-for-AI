# Prompt Input Design

## What
Prompt Input Design helps users give an AI system enough context, constraints, and intent to produce useful results.

The interface should make good prompting easier without requiring prompt expertise.

## Why it matters
AI output quality depends heavily on input quality.

Good prompt input design:
- improves output relevance
- reduces user frustration
- prevents blank-page anxiety
- guides constraints
- makes AI features feel more reliable

Users should not need to become prompt engineers to get value.

## When to apply
- AI text generation
- design generation
- code generation
- research tools
- AI agents
- summarisation
- recommendation systems
- prompt builders

## How to apply

- ask for the user's goal first
- provide structured fields when context matters
- offer examples or templates without overwhelming
- make constraints easy to specify
- preserve and reuse useful context
- let users refine inputs after seeing output

The input should guide the user toward a high-quality request.

## Implementation rules

- input must clarify the desired outcome
- required context must be explicit
- examples must match real user tasks
- constraints must be easy to add or edit
- prompt history or drafts should be preserved where useful
- empty input states must guide action

## Example

Bad:
- blank textarea with "Ask AI"
- no examples
- asks for too much context at once
- user cannot revise the prompt after output

Good:
- goal field plus optional constraints
- relevant prompt examples
- saved context from the project
- easy refine-and-regenerate path

## Fail conditions

- user does not know what to enter
- output quality fails because needed context was not requested
- examples are generic or misleading
- prompt editing is difficult
- user loses prompt work

## Enforcement rule

If AI output depends on user context, design the input so a non-expert can provide that context clearly.

