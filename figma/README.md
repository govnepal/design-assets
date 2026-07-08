# design-figma

Bridge between the Figma library and the rest of the system. Figma files live in Figma;
this repo makes the library versioned and auditable.

- `tokens-sync/` — Tokens Studio config pointed at design-guidelines DTCG token JSON
- `mapping/` — component-name map: "Button / Primary" ↔ `button` id
- `library/` — CHANGELOG.md per published library version + structure.md (§17.1 pages)
- `exports/` — periodic token/style exports for audit diffing

Direction of truth: design-guidelines → Figma (tokens/content); Figma owns visual craft.
