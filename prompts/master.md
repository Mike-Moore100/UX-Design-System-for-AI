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
2. active module rule files: `UX.md` and `DESIGN.md`
3. `methods/index.md`
4. relevant files in `methods/ux/`
5. relevant files in `methods/design/`
6. `scorecard.md`
7. `layr.config.md`, if present
8. relevant screen brief in `/screens`, if present

Treat Layr files as strict rules, not suggestions.

Apply active modules only.
Do not treat planned modules as complete Layr systems until their rule files and methods exist.

---

## Context Policy

Do not require the user to edit Layr files before using the system.

Use context in this order:

1. the user's task
2. the existing codebase or product
3. `layr.config.md`, if present
4. screen briefs in `/screens`, if present

If context is missing, infer the most likely user, goal, and primary action.

Ask at most 3 questions only when the missing information would materially change the UX direction.
Otherwise proceed and state assumptions briefly.

---

## Process

1. Define the screen, user intent, primary goal, and primary action.
2. Select relevant UX and design methods using `methods/index.md`.
3. Apply `UX.md` and `DESIGN.md` as strict constraints.
4. Preserve the existing product design language unless the task asks for a redesign.
5. Build or improve the UI.
6. Score the result with `scorecard.md`.
7. Fix weak areas.
8. Repeat until the score is at least 85.

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
2. UX score `/100`
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
