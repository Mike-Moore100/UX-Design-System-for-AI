# Master Prompt

Use the Layr system to build, review, or improve UI.

Primary instruction:

```text
Read RUN.md first, then follow it.
```

If RUN.md is not available, follow this prompt directly.

---

## Load Order

Read these files in order:

1. `modules/index.md`
2. active module rule files relevant to the task
3. `methods/index.md`
4. relevant method files
5. `scorecard.md`
6. `layr.config.md`, if present
7. relevant screen brief in `/screens`, if present

Treat Layr files as strict rules, not suggestions.

Apply only the modules that materially improve the current task.
Respect `Scope:` and `Depth:` when the user provides them.
If they are missing, use `Scope: Auto` and `Depth: Standard`.

---

## Scope And Depth

Use `Scope:` to choose modules.
Use `Depth:` to choose how much of Layr to apply.

Supported scope values:

- `Auto`
- `UX`
- `Design`
- `Accessibility`
- `Security`
- `Performance`
- `Analytics`
- `QA`
- `AI Product`
- `CRO`
- `SEO`
- `AI Search`
- `Marketing`
- `Copywriting`

`AI Search` maps to SEO and specifically includes `methods/seo/ai-search-visibility.md`.

Supported depth values:

- `Quick` - 2-4 methods
- `Standard` - 4-8 methods
- `Deep` - 8-14 methods

Do not load the whole method library unless the user asks for a full audit.

---

## Context Policy

Do not require the user to edit Layr files before using the system.

Use context in this order:

1. the user's task
2. explicit `Scope:` and `Depth:`, if provided
3. optional context block in the prompt, if provided
4. the existing codebase or product
5. `layr.config.md`, if present
6. screen briefs in `/screens`, if present

If context is missing, infer the most likely user, goal, and primary action.

Ask at most 3 questions only when the missing information would materially change the product direction.
Otherwise proceed and state assumptions briefly.

---

## Process

1. Define the screen, user intent, primary goal, and primary action.
2. Read the user's `Scope:` and `Depth:` values, or use the defaults.
3. Select relevant modules using `modules/index.md`.
4. Select relevant methods using `methods/index.md` within the chosen depth.
5. Apply relevant module rule files as strict constraints.
6. Preserve the existing product design language unless the task asks for a redesign.
7. Build or improve the UI.
8. Score the result with `scorecard.md`.
9. Fix weak areas.
10. Repeat until the score is at least 85.

---

## Non-Negotiables

- one primary action per screen
- no competing primary actions
- no unnecessary decisions
- no decorative elements that reduce clarity
- no random design decisions
- no inconsistent patterns
- no weak hierarchy
- no inaccessible interaction states

Everything must feel structured, intentional, predictable, and effortless.

---

## Output

Return only:

1. final improved solution
2. Layr score `/100`
3. key improvements made
4. assumptions, only if context was inferred

Do not return first drafts.
Do not return multiple options unless the user asks.
Do not expose chain-of-thought reasoning.

---

## Final Rule

The system must produce UI that reduces friction, builds trust, and drives action.

If the user hesitates, it failed.
If the user has to think, it failed.
