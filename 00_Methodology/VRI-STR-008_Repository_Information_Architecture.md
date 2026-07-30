---
title: Repository Information Architecture
id: VRI-STR-008
jurisdiction: Multi-state (Veridion institutional)
citation: Internal strategy
regulatory_topic: Knowledge architecture
agency: Veridion
license_types: N/A
effective_date: 2026-07-30
last_reviewed: 2026-07-30
risk_level: Foundational
related_nodes:
  - VRI-STR-009_BikeMN_Knowledge_Ethos
  - VRI-STR-007_The_Content_Flywheel
  - VRI-STR-006_Atomic_Knowledge_Architecture
status: Active
---

# VRI-STR-008
# Repository Information Architecture

Status: Active

## Authority

Internal Veridion strategy document defining the canonical directory structure, naming conventions, and navigation philosophy for VRN RegMatrix.

## Intent

To keep the knowledge base navigable as it scales, prevent folder sprawl, and ensure every directory remains self-documenting.

## Plain Language Summary

Folders hold categories. Knowledge nodes hold ideas. People should move primarily by following links, not by digging deeper into nested folders. Every folder explains itself.

## Operational Meaning

- Use the numbered top-level directories listed below.
- Prefer concept names over project or version names.
- Require a README in every directory.
- Link densely; do not rely on deep folder hierarchy for discovery.

## Enforcement Considerations

New top-level directories outside the canonical list require explicit amendment of this document. Unexplained directories or files without READMEs are incomplete.

## Common Failure Points

- Creating project-named folders (e.g., "ClientX_Final_v3")
- Deep nesting that hides content
- Missing READMEs
- Duplicate content across folders instead of linking

## Related Regulations / Nodes

- Upstream: VRI-STR-009 Knowledge Ethos
- Downstream: All content directories
- Related: VRI-STR-006 (node structure), VRI-STR-007 (flywheel outputs map to these folders)

## Related Context Maps

- Migration from prior Hexa_Spire / ClearLine structures

## Related Action Maps

- Directory creation checklist (future)

## Sources

- Observed friction in prior multi-vault and multi-repo knowledge production
- Atomic knowledge design principles

## Canonical Structure

```
00_Methodology
01_Reg_Bibles
02_Reg_Pol_Notebooks
03_Playbooks
04_Penumbrant_Papers
05_Context_Maps
06_Action_Maps
07_Case_Studies
08_FAQs
09_Glossary
resources
```

## Directory Rules

Folders organize categories.

Knowledge nodes organize ideas.

Navigation should occur primarily through links rather than folder depth.

## Naming

Names should describe concepts rather than projects.

Prefer:

Inventory Audits

instead of

InventoryAudit_Final_v7

## README Requirement

Every directory SHALL contain a README explaining:

- purpose
- contents
- relationships
- contribution expectations
