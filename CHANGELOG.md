# Changelog

All notable changes to Layr are documented here.

Use this file as the in-repo version history.
Use GitHub Releases for public tagged releases.

---

## [1.3.0] - 2026-05-09

### Added

- Added 10 additional methods to each active Layr category: UX, Design, Accessibility, Security, CRO, SEO, Marketing, and Copywriting.
- Added `methods/seo/ai-search-visibility.md` for AI answer, ChatGPT search, Copilot, GEO, and answer-engine visibility.
- Added active Performance, Analytics, QA, and AI Product module rule files.
- Added 5 launch-critical methods each for Performance, Analytics, QA, and AI Product.
- Added `Scope:` and `Depth:` controls so users can invoke only the modules and method depth they need.
- Expanded `methods/index.md` so AI tools can route across the full method library by category, surface type, and problem type.

### Changed

- Strengthened method routing for landing pages, onboarding, pricing, forms, public content, sensitive flows, vague copy, hesitation points, audience scaling, and unfinished interface states.
- Updated README, RUN, master prompt, and AI-tool entry files to default to `Scope: Auto` and `Depth: Standard`.
- Expanded optional context fields without making setup mandatory.
- Moved active module rule files into `modules/` so the repository root stays easier to scan.

---

## [1.2.0] - 2026-05-09

### Added

- Added active Accessibility, Security, CRO, SEO, Marketing, and Copywriting module rule files.
- Added 5 methods each for Accessibility, Security, CRO, SEO, Marketing, and Copywriting.
- Updated `methods/index.md` to route across all active production modules.
- Updated `scorecard.md` from UX-only scoring to modular Layr scoring.

### Changed

- Split methods into `methods/ux/` and `methods/design/`.
- Updated `methods/index.md` to route AI tools between UX methods and design methods.
- Moved visual design methods into `methods/design/`.
- Expanded the module routing layer across all active Layr modules.
- Added design-specific methods for colour theory, typography, spacing rhythm, layout composition, contrast and emphasis, component consistency, and motion clarity.
- Added `modules/index.md` to define active modules and selection rules.
- Added `ROADMAP.md` to describe the future module direction.

---

## [1.1.0] - 2026-05-09

### Changed

- Replaced manual placeholder setup with a zero-setup flow.
- Added `RUN.md` as the main AI entry point.
- Updated the README to support repo URL usage first and local folder usage second.
- Made `layr.config.md` optional instead of required.
- Made screen briefs optional instead of required.
- Updated `modules/ux.md` and `modules/design.md` so users do not edit core rule files.
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
- `modules/ux.md` for behaviour, flow, scoring, and validation.
- `modules/design.md` for hierarchy, spacing, layout, and visual clarity.
- UX methods library covering Fitts's Law, Hick's Law, Cognitive Load, Jakob's Law, Gestalt, Signal to Noise, Default Bias, and more.
- Master prompt in `/prompts`.
- Screen definition template.
- Before and after examples.
