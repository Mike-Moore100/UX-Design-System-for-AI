# AI Features Playbook

Use this playbook for generation, retrieval, recommendations, agents, automation, and reviewable generated output.

---

## Required Modules

- AI Product
- UX
- Design
- Accessibility
- Security, when data or actions are sensitive
- Performance, when responses are slow, streamed, or long-running
- Analytics, when adoption, quality, or correction needs must be measured
- QA
- Copywriting, for input guidance, uncertainty, errors, and review copy

---

## Recommended Methods

- `methods/ai/prompt-input-design.md`
- `methods/ai/output-trust.md`
- `methods/ai/human-control.md`
- `methods/ai/ai-fallbacks.md`
- `methods/ai/ai-evaluation.md`
- `methods/security/data-minimisation.md`
- `methods/performance/loading-strategy.md`
- `methods/analytics/privacy-aware-analytics.md`
- `methods/qa/edge-case-states.md`

---

## Hard Gates

- user understands what the feature can and cannot do
- input guidance improves output quality
- generated output is reviewable before high-impact use
- uncertainty or limits are visible when they affect decisions
- user can edit, retry, reject, or undo
- sensitive data handling is clear and minimal
- loading, failure, refusal, and partial-output states exist
- quality feedback or evaluation path exists when relevant

---

## Production Rules

- Set expectations before generation begins.
- Ask for the minimum useful input.
- Show progress for long-running work.
- Make output sources, assumptions, or limits visible when they affect trust.
- Keep user approval before irreversible or sensitive actions.
- Provide correction paths that do not require starting over.
- Avoid logging prompts, outputs, or sensitive context unless needed and permitted.
- Track usage, retries, edits, acceptance, rejection, and failure when measurement is in scope.

---

## Common Failure Patterns

- feature promises more certainty than it can provide
- user cannot shape the input
- output replaces user work without review
- failure state is a generic error
- retry repeats the same bad result
- sensitive information is requested without explanation
- quality is not measurable

---

## Evidence Required Before Scoring

- input design helps the user provide useful context
- output is reviewable, editable, and rejectable
- uncertainty, source, or limitation cues appear when needed
- fallback and failure states are present
- sensitive data is minimized and explained
- feedback or evaluation loop exists when quality matters
