# Layr Agent Instructions

When a user asks to use Layr, read `RUN.md` first and follow it.

Do not ask the user to edit Layr files before starting.
Do not require `layr.config.md` or a screen brief.

Use the zero-setup flow by default:

1. infer product context from the task and codebase
2. use `Scope: Auto` and `Depth: Standard` unless the user specifies otherwise
3. read `modules/index.md`, relevant module rule files, `methods/index.md`, relevant methods, and `scorecard.md`
4. ask at most 3 questions only when missing context would materially change the product direction
5. implement or return the improved UI
6. score the result with evidence

Preserve existing design systems unless the user explicitly asks for a redesign.
Apply only the Layr modules that materially improve the task.
Respect explicit `Scope:` and `Depth:` values when provided.
