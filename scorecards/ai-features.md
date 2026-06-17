# AI Features Scorecard

Score generation, retrieval, recommendations, agents, automation, and reviewable generated output out of 100.

---

## Categories

- Input clarity: 0-15
- Output trust and reviewability: 0-15
- User control and correction: 0-15
- Safety, privacy, and data minimisation: 0-15
- Loading, failure, and fallback states: 0-10
- Accessibility and interaction quality: 0-10
- Quality measurement: 0-10
- QA and edge-state coverage: 0-10

---

## Hard Cap Rules

The feature cannot score above 84 if:

- users cannot understand what the feature can and cannot do
- generated output is not reviewable before high-impact use
- users cannot edit, retry, reject, or undo
- sensitive data handling is unclear
- failure states are missing

The feature cannot score above 70 if:

- output can trigger sensitive or irreversible action without review
- user input has no guidance
- quality cannot be evaluated where quality matters

---

## Evidence Required

- input guidance helps users provide useful context
- output is reviewable, editable, rejectable, or reversible
- uncertainty, limits, or evidence appear where trust depends on them
- fallback, failure, and partial-output states are handled
- sensitive data requests are minimized and explained
- feedback or evaluation loop exists when product quality depends on output quality
