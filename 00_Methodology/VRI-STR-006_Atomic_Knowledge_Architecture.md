---
title: Atomic Knowledge Architecture
id: VRI-STR-006
jurisdiction: Multi-state (Veridion institutional)
citation: Internal strategy
regulatory_topic: Knowledge node design
agency: Veridion
license_types: N/A
effective_date: 2026-07-30
last_reviewed: 2026-07-30
risk_level: Foundational
related_nodes:
  - VRI-STR-009_BikeMN_Knowledge_Ethos
  - VRI-STR-008_Repository_Information_Architecture
  - VRI-STR-007_The_Content_Flywheel
status: Active
---

# VRI-STR-006
# Atomic Knowledge Architecture

Status: Active

## Authority

Internal Veridion strategy document defining the unit of organization, required metadata, required sections, linking rules, and anti-duplication rule for every knowledge node in RegMatrix.

## Intent

To make regulatory knowledge behave like a web rather than a filing cabinet so that AI systems, human researchers, and future products can traverse, recombine, and trust the information.

## Plain Language Summary

Documents are not the unit. Knowledge nodes are. Each regulation (or coherent regulatory concept) becomes a node with consistent metadata and sections. Nodes link to each other. Information is written once and referenced everywhere else.

## Operational Meaning

- Create or update a knowledge node rather than a free-form document whenever possible.
- Populate the required metadata fields.
- Include the required sections (or explicitly mark them N/A with reason).
- Satisfy the linking rules before considering the node complete.
- Never copy substantive content; link instead.

## Enforcement Considerations

Nodes missing required metadata or sections, or that duplicate content instead of linking, are incomplete. Automated or human review should surface these gaps.

## Common Failure Points

- Treating a long PDF-style memo as a finished knowledge product
- Copy-pasting the same statutory summary into multiple places
- Orphan nodes with no upstream or downstream links
- Inconsistent metadata fields that break filtering or AI retrieval

## Related Regulations / Nodes

- Upstream: VRI-STR-009 and VRI-STR-008
- Downstream: Every content node in the repository
- Related: VRI-STR-007 (the flywheel produces these nodes)

## Related Context Maps

- Node schema and template (to be placed in resources/)

## Related Action Maps

- Node creation checklist (future)

## Sources

- Atomic design and knowledge graph principles adapted to regulatory domains
- Practical experience with multi-state cannabis regulatory research under ClearLine / Veridion

## Principle

Every regulation SHALL become a knowledge node.

Documents are not the unit of organization.

Knowledge nodes are.

## Required Metadata

Every knowledge node SHOULD contain:

- Title
- Jurisdiction
- Citation
- Regulatory Topic
- Agency
- License Types
- Effective Date
- Last Reviewed
- Risk Level
- Related Nodes

## Required Sections

Authority  
Intent  
Plain Language Summary  
Operational Meaning  
Enforcement Considerations  
Common Failure Points  
Related Regulations  
Related Context Maps  
Related Action Maps  
Sources

## Linking Rules

Every page SHALL link to:

- one upstream authority
- one downstream operational artifact
- at least three related nodes

Knowledge should behave like a web instead of a filing cabinet.

## Duplication Rule

Information should exist once.

Other pages reference it.

They do not copy it.
