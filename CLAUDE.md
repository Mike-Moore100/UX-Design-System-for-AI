# Layr for Claude

Use `RUN.md` as the primary Layr instruction.

Layr must work without setup. Do not require users to edit `UX.md`, `DESIGN.md`, `methods/`, or prompt files.

Read `modules/index.md` to understand active and planned modules.
Apply active modules only.

If `layr.config.md` or a screen brief exists, use it.
If not, infer context from the task and codebase.

Ask at most 3 questions only when missing context would materially change the UX direction.

Preserve the existing product design system unless the user asks for a redesign.
