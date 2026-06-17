# Run Layr

Use this file after `SYSTEM.md` as the main execution entry point for Layr.

Layr must work with zero setup, then improve when optional context is available.

---

## Fastest Use

If the user provides only a task, proceed.

Do not ask them to fill templates before work begins.
Do not require edits to `SYSTEM.md`, module files, `methods/`, or this file.

Default to:

```text
Scope: Auto
Depth: Standard
```

---

## Load Order

Read these files in order:

1. `SYSTEM.md`
2. `playbooks/index.md`
3. relevant surface playbook in `playbooks/`
4. `modules/index.md`
5. active module rule files in `modules/` relevant to the task
6. `methods/index.md`
7. relevant method files
8. `scorecard.md`
9. relevant surface scorecard in `scorecards/`, if present
10. `layr.config.md`, if present
11. relevant screen brief in `/screens`, if present

If working from the GitHub repo URL, fetch the same files from the repository before applying the system.

---

## Scope Control

Users may control which parts of Layr run by adding `Scope:` to the prompt.

If no scope is provided, use `Scope: Auto`.

Supported scope values:

- `Auto` - infer the smallest relevant module set from the task
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
- any comma-separated combination of the above

Examples:

```text
Scope: UX, CRO, Copywriting
```

```text
Scope: SEO, AI Search
```

Scope rules:

- do not run every module unless the user asks for a full audit
- if the user provides explicit scope, respect it
- add a missing module only when it is required to avoid a serious quality, safety, accessibility, or implementation failure
- if adding a missing module, state the assumption briefly
- `AI Search` maps to SEO and specifically includes `methods/seo/ai-search-visibility.md`

---

## Depth Control

Users may control how deeply Layr runs by adding `Depth:` to the prompt.

If no depth is provided, use `Depth: Standard`.

Supported depth values:

- `Quick` - use 2-4 methods, focus on the biggest visible issue
- `Standard` - use 4-8 methods, suitable for normal product work
- `Deep` - use 8-14 methods, suitable for important screens, audits, launches, SEO, security, AI features, performance-critical paths, or conversion-critical flows

Depth rules:

- never load the whole method library by default
- load only the selected module files
- load only method files that materially affect the task
- use deeper analysis only when requested or when the surface is high risk

---

## Module Policy

Apply only the modules that materially improve the current task.

Current active modules:

- UX
- Design
- Accessibility
- Security
- Performance
- Analytics
- QA
- AI Product
- Conversion Rate Optimisation
- SEO
- Marketing
- Copywriting

`AI Search` is an SEO scope, not a separate module.

Default for product UI:

1. UX
2. Design
3. Accessibility

Add specialist modules only when the surface requires them.
Use `modules/index.md` and `methods/index.md` to route the task.

---

## Context Policy

Use context in this order:

1. the user's task
2. explicit `Scope:` and `Depth:`, if provided
3. optional context block in the prompt, if provided
4. the existing codebase or product
5. `layr.config.md`, if present
6. screen briefs in `/screens`, if present

Infer missing context when it is reasonably clear.

Ask at most 3 questions only when missing information would materially change the product direction, such as:

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
Use `Scope: Auto` and `Depth: Standard` unless the user specifies otherwise.

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

1. Define the surface type, user intent, primary goal, and primary action.
2. Read the user's `Scope:` and `Depth:` values, or use the defaults.
3. Use `SYSTEM.md` to identify hard gates and conflict rules.
4. Load the relevant surface playbook from `playbooks/`.
5. Select relevant modules using `modules/index.md`.
6. Select relevant methods using `methods/index.md` within the chosen depth.
7. Apply active module rule files from `modules/` as strict constraints.
8. Preserve the existing design language unless the task explicitly asks for a redesign.
9. Build or improve the UI.
10. Score the result with `scorecard.md` and the relevant surface scorecard when present.
11. Fix weak areas.
12. Repeat until the score is at least 85.

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
2. Layr score `/100`
3. selected playbook, when used
4. selected modules and methods
5. hard gates checked
6. key improvements made
7. assumptions, only when context was inferred

For code tasks, implement the change directly when possible.

Do not return first drafts.
Do not return multiple options unless the user asks.
Do not expose chain-of-thought reasoning.

---

## Final Rule

Layr exists to remove friction without reducing quality.

The best result is fast to use, easy to understand, visually consistent, and immediately actionable.
