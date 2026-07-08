# design-fonts

Font packages for the design system: Devanagari + Latin.

- `fonts/` — woff2 per family/weight (incl. Noto Sans Devanagari or approved family)
- `subsets/` — subsetting configs/scripts
- `css/` — @font-face stylesheets + fallback stacks
- `test/` — Nepali rendering / line-height test pages (Devanagari needs more line-height)
- `LICENSES/` — per-family license files

Ships as an npm package / CDN bundle consumed by design-web and referenced by design-figma.
