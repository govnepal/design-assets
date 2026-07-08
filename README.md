# design-assets

All design assets for the Nepal Digital Design System: icons, fonts, emblems,
illustrations, photos, animations, and the Figma bridge.

## Structure

- `icons/` — official icon set: `src/` one optimized SVG per icon + `meta/` YAML (contribute: one SVG + one YAML in a PR)
- `fonts/` — Devanagari + Latin font packages, subsetting, @font-face CSS, rendering test pages
- `emblems/` — official emblem/flag/map masters (restricted license, never modified without government liaison)
- `illustrations/`, `photos/`, `animations/` — asset catalog: metadata YAML in git; large binaries move to object storage + CDN when needed (none yet)
- `figma/` — Figma library bridge: tokens-sync config, name↔spec-id mapping, library changelog

`icons/`, `fonts/`, and `figma/` were separate repos (design-icons, design-fonts,
design-figma) in the full architecture; consolidated here while the team is small.
See "Current phase" in design-web/docs/repo-structure.md.

## Rules

- Every asset has metadata: title/title_ne, license, status (official | community | under-review), contributor.
- Icon/asset metadata validates against schemas in design-guidelines.
- MIT covers the repo code/metadata; per-asset licensing is in LICENSES.md (emblems restricted).
