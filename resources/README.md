# resources

## Purpose

Primary sources, templates, schemas, agent prompts, and supporting materials that the knowledge nodes reference or that enable consistent production and cross-repo projection.

## Contents

| File | Purpose |
|------|--------|
| `node_template.md` | Canonical front-matter + required sections for every knowledge node |
| `public_projection_template.md` | Thin public-facing shape used when projecting a node into CLRegMatrix |
| (future) Research session / flywheel checklist |
| (future) Citation style guide |
| (future) Primary source indexes by jurisdiction |
| (future) Agent / system prompts |

## Relationships

- Upstream: `00_Methodology/` (especially VRI-STR-006, VRI-STR-010)
- Downstream: All content production and the projection workflow in `.github/workflows/`
- Public product site: CLRegMatrix uses the projection template and must always link back here

## Contribution Expectations

- Templates must remain lightweight and enforceable
- Primary sources should be indexed, not wholesale duplicated when possible
- Keep agent/system prompts versioned and linked to the methodology that governs them
- Any change to `node_template.md` should be reflected in existing nodes over time
