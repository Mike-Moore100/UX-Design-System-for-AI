# Run Layr

Use this file as the main entry point for Layr.

Layr must work with zero setup, then improve when optional context is available.

---

## Fastest Use

If the user provides only a task, proceed.

Do not ask them to fill templates before work begins.
Do not require edits to `UX.md`, `DESIGN.md`, `/methods`, or this file.

---

## Load Order

Read these files in order:

1. `UX.md`
2. `DESIGN.md`
3. `methods/index.md`
4. relevant files in `/methods`
5. `scorecard.md`
6. `layr.config.md`, if present
7. relevant screen brief in `/screens`, if present

If working from the GitHub repo URL, fetch the same files from the repository before applying the system.

---

## Context Policy

Use context in this order:

1. the user's task
2. the existing codebase or product
3. `layr.config.md`, if present
4. screen briefs in `/screens`, if present

Infer missing context when it is reasonably clear.

Ask at most 3 questions only when missing information would materially change the UX direction, such as:

- the primary user is ambiguous
- the primary action is ambiguous
- the screen's success criteria are ambiguous
- brand or design constraints conflict with the requested change

If the missing detail would only refine the result, proceed with a clear assumption.

---

## Quality Modes

### Zero Setup

Use when the user wants speed.

Required input:

```text
Task:
```

Infer product context from the repo and task.

### Recommended

Use when the user wants stronger product fit.

Read `layr.config.md` if it exists.
If it does not exist, continue without it.

### Screen-Level

Use when the user wants maximum precision for an important screen.

Read the relevant screen brief in `/screens` if it exists.
If no screen brief exists, infer the screen intent from the task and codebase.

---

## Execution

For every task:

1. Define the screen, user intent, primary goal, and primary action.
2. Select relevant methods using `methods/index.md`.
3. Apply `UX.md` and `DESIGN.md` as strict constraints.
4. Preserve the existing design language unless the task explicitly asks for a redesign.
5. Build or improve the UI.
6. Score the result with `scorecard.md`.
7. Fix weak areas.
8. Repeat until the score is at least 85.

---

## Design Preservation

If the product already has a design system:

- use existing tokens, components, spacing, typography, and interaction patterns
- do not introduce a new visual style
- do not restyle unrelated areas
- only change what improves clarity, usability, hierarchy, accessibility, or task completion

If no design system exists:

- use accessible neutral defaults
- create a small, consistent visual system
- avoid decorative style choices that do not improve usability

---

## Output

Return only:

1. final improved solution
2. UX score `/100`
3. key improvements made
4. assumptions, only when context was inferred

For code tasks, implement the change directly when possible.

Do not return first drafts.
Do not return multiple options unless the user asks.
Do not expose chain-of-thought reasoning.

---

## Final Rule

Layr exists to remove friction without reducing quality.

The best result is fast to use, easy to understand, visually consistent, and immediately actionable.
