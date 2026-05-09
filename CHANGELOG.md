# Changelog

All notable changes to Layr are documented here.

Use this file as the in-repo version history.
Use GitHub Releases for public tagged releases.

---

## [1.2.0] - 2026-05-09

### Changed

- Split methods into `methods/ux/` and `methods/design/`.
- Updated `methods/index.md` to route AI tools between UX methods and design methods.
- Moved visual design methods into `methods/design/`.
- Added a module routing layer for active and planned Layr modules.

### Added

- Added design-specific methods for colour theory, typography, spacing rhythm, layout composition, contrast and emphasis, component consistency, and motion clarity.
- Added `modules/index.md` to define active modules and planned modules.
- Added `ROADMAP.md` to describe the future module direction.

---

## [1.1.0] - 2026-05-09

### Changed

- Replaced manual placeholder setup with a zero-setup flow.
- Added `RUN.md` as the main AI entry point.
- Updated the README to support repo URL usage first and local folder usage second.
- Made `layr.config.md` optional instead of required.
- Made screen briefs optional instead of required.
- Updated `UX.md` and `DESIGN.md` so users do not edit core rule files.
- Added evidence-based scoring through `scorecard.md`.
- Added `methods/index.md` so AI tools can choose relevant methods instead of applying everything.
- Added AI-tool entry files for Codex, Claude, and Cursor.
- Normalized method and screen folders to lowercase paths.

### Fixed

- Removed outdated setup instructions that required users to paste multiple files manually.
- Removed references to obsolete website-based setup.
- Fixed incorrect path references such as `/templates/screen.md`.
- Fixed inconsistent file casing in instructions.

---

## [1.0.0] - Previous

### Added

- Initial Layr UX and design rule system.
- `UX.md` for behaviour, flow, scoring, and validation.
- `DESIGN.md` for hierarchy, spacing, layout, and visual clarity.
- UX methods library covering Fitts's Law, Hick's Law, Cognitive Load, Jakob's Law, Gestalt, Signal to Noise, Default Bias, and more.
- Master prompt in `/prompts`.
- Screen definition template.
- Before and after examples.
