# AGENTS.md — design-assets

All design assets: icons/ (SVG + meta YAML; run svgo; use currentColor; follow the iconography-style chapter), fonts/ (woff2 only, no thin weights, respect OFL licenses, Nepali needs more line-height), figma/ (direction of truth: guidelines → Figma), emblems (masters IN git, restricted), illustrations/photos/animations (meta YAML catalog in git; large binaries go to object storage + CDN when needed — none yet). No Git LFS.

## Rules
- NEVER modify emblem/flag/map masters — they are legally controlled; changes require the government liaison.
- Every asset has a meta YAML: title/title_ne, license, status (official | community | under-review), contributor; bucket files also need storage_key, checksum, sizes.
- CI is the only writer to the bucket. Binaries go to the staging prefix; merge promotes them. Never hand-upload to the public prefix.
- Do not commit photos/videos/large sources to git — metadata only.

## Ecosystem rules (all govnepal design repos)

- This is part of the Nepal Digital Design System (Civic Calm) — an unofficial, community-led initiative. See design-web/docs/repo-structure.md for the full architecture.
- `design-guidelines` is the single source of truth. Consume other repos by git TAG, never by main.
- Everything is bilingual: every title/label field has a `_ne` (Nepali) counterpart. If you add a field with user-facing text, add `_ne` too (value `TODO` if you cannot translate).
- Accessibility target is WCAG 2.2 AA. Never communicate status by color alone; keep visible labels and focus states.
- Never hardcode visual values (hex colors, px spacing) in product code — use semantic tokens.
- `id` fields are permanent once published. Rename titles freely; never change ids.
- Commit style: short imperative subject; no scope prefixes.
