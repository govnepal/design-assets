# design-icons

Official icon set for the Nepal Government Digital Design Guidelines.

- `src/` — one optimized SVG per icon (svgo), named by id: `passport.svg`, `ward.svg`
- `meta/` — one YAML per icon: id, name, name_ne, category, tags, status, contributor
  (validates against the schema in design-guidelines)
- `scripts/` — optimize, build sprite / npm package / depot catalog bundle

Icons must follow the `iconography-style` chapter of the guidelines
(grid, stroke weight, corner radius, filled/outline, metaphor rules).

**Contribute an icon:** one SVG + one YAML in a PR.
