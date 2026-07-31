---
title: Cross-Repo Linking and Sync Rules
id: VRI-STR-010
jurisdiction: Multi-state (Veridion institutional)
citation: Internal strategy
regulatory_topic: Knowledge architecture / publishing
agency: Veridion
license_types: N/A
effective_date: 2026-07-31
last_reviewed: 2026-07-31
risk_level: Foundational
public_status: ready
related_nodes:
  - id: VRI-STR-006
    path: 00_Methodology/VRI-STR-006_Atomic_Knowledge_Architecture.md
    relation: methodology
  - id: VRI-STR-008
    path: 00_Methodology/VRI-STR-008_Repository_Information_Architecture.md
    relation: methodology
  - id: VRI-STR-009
    path: 00_Methodology/VRI-STR-009_BikeMN_Knowledge_Ethos.md
    relation: methodology
status: Active
---

# VRI-STR-010
# Cross-Repo Linking and Sync Rules

Status: Active

## Authority

Internal Veridion strategy governing the relationship between the institutional knowledge bank (VRN-RegMatrix) and the public product site (CLRegMatrix).

## Intent

Preserve a clean separation of concerns while ensuring the public face always points back to the single source of truth and that information is never duplicated as independent content.

## Plain Language Summary

VRN-RegMatrix owns the knowledge. CLRegMatrix shows selected, simplified views of that knowledge. Links are directional and explicit. Automation helps move content one way (VRN → public) under human review.

## Operational Meaning

### Roles

- **VRN-RegMatrix** = Source of truth, full nodes, methodology, flywheel outputs, internal depth.
- **CLRegMatrix** = Public-facing product site: simple state offerings, doctrine overview, polished or progressive projections.

### Linking Rules

1. Every public page that contains substantive regulatory content MUST include a visible “Source of truth” block linking to the corresponding VRN node(s) or directory.
2. VRN nodes MAY optionally declare a `public_projection` URL once a public page exists.
3. Prefer stable node `id` values and concept-based filenames.
4. Cross-repo links use absolute GitHub or GitHub Pages URLs.
5. Intra-VRN links follow VRI-STR-006 (upstream, downstream, ≥3 related).

### Public Status Field

Nodes carry `public_status`:

- `internal` — not for public projection
- `draft` — work in progress
- `ready` — eligible for projection / sync
- `published` — has a live public page

Only `ready` or `published` nodes should be candidates for automated or manual projection.

### Sync Philosophy

- One-way preferred: VRN → CLRegMatrix.
- Human review gate (PR) before public main is updated.
- No silent overwrites of the public site.
- Manifest or front-matter tracks what has been projected and when.

## Enforcement Considerations

- Duplicated substantive content across the two repos is a violation of the Atomic Knowledge Architecture.
- Missing source-of-truth links on public pages degrade trust and discoverability of the deeper bank.
- Automation that writes directly to public `main` without review is discouraged.

## Common Failure Points

- Copy-pasting full node content into CLRegMatrix instead of projecting a thin summary.
- Public pages that drift and are no longer linked to any living VRN node.
- Treating the two repos as independent authoring surfaces.

## Related Regulations / Nodes

- Upstream: VRI-STR-006, VRI-STR-008, VRI-STR-009
- Downstream: resources/node_template.md, resources/public_projection_template.md, .github/workflows/

## Related Context Maps

- Overall Veridion / TVK knowledge system architecture (broader personal + product OS)

## Related Action Maps

- Post-research projection checklist (future)
- Sync validation script (future)

## Sources

- Decision log 2026-07-30/31: keep public face simple; wiring lives in VRN Node.
- VRI-STR-006 through 009.

## Implementation Notes

See `resources/` for templates and `.github/workflows/` for the projection workflow.
