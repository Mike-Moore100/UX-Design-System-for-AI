# Layr for Claude

Use `RUN.md` as the primary Layr instruction.

Layr must work without setup. Do not require users to edit module files, `methods/`, or prompt files.

Read `modules/index.md` to choose relevant modules.
Apply only the Layr modules that materially improve the task.
Use `Scope: Auto` and `Depth: Standard` unless the user specifies otherwise.
Respect explicit `Scope:` and `Depth:` values when provided.

If `layr.config.md` or a screen brief exists, use it.
If not, infer context from the task and codebase.

Ask at most 3 questions only when missing context would materially change the product direction.

Preserve the existing product design system unless the user asks for a redesign.
