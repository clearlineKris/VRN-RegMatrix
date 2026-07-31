# VRN RegMatrix

**Veridion Regulatory Matrix**  
The living institutional knowledge base for multi-state cannabis regulatory intelligence.

Formerly CLRegMatrix / ClearLine RegMatrix.  
Status: Active foundational build (2026-07-31)

This repository is one operational pillar within the broader **TVK / Veridion knowledge system** (personal OS + product intelligence). It is deliberately structured so that any reader — collaborator, future self, or agent — can understand the rules, contribute consistently, and follow the links without tribal knowledge.

---

## Purpose

VRN RegMatrix exists to become a trusted source of regulatory understanding.

Authority is earned through consistently useful public knowledge.

The repository answers questions before clients ask them.  
It educates before it sells.  
Consulting is an application of the knowledge bank — not its purpose.

---

## Canonical Structure

Per **VRI-STR-008 Repository Information Architecture**:

| Directory | Purpose |
|-----------|---------|
| `00_Methodology` | Strategic principles, atomic architecture, contribution rules, flywheel, cross-repo rules |
| `01_Reg_Bibles` | Statutory authority organized by jurisdiction and domain |
| `02_Reg_Pol_Notebooks` | Policy analysis, legislative history, stakeholder maps |
| `03_Playbooks` | Operational procedures and field guidance |
| `04_Penumbrant_Papers` | Gray-zone risk analysis (penumbral zones) |
| `05_Context_Maps` | Timeline, economic, enforcement climate, cross-state context |
| `06_Action_Maps` | Decision trees and operational response maps |
| `07_Case_Studies` | Enforcement narratives and lessons |
| `08_FAQs` | Practical Q&A derived from research |
| `09_Glossary` | Defined terms with citations |
| `resources` | Templates, schemas, supporting materials |
| `.github/workflows` | Projection / sync automation |

Folders organize categories.  
Knowledge nodes organize ideas.  
Navigation occurs primarily through links rather than folder depth.

---

## Core Principles (Active)

- **[VRI-STR-009] BikeMN Knowledge Ethos** — Trusted source; educate before sell
- **[VRI-STR-008] Repository Information Architecture** — Canonical structure & naming
- **[VRI-STR-007] The Content Flywheel** — Research produces multiple reusable assets
- **[VRI-STR-006] Atomic Knowledge Architecture** — Every regulation becomes a knowledge node
- **[VRI-STR-010] Cross-Repo Linking and Sync Rules** — Public face vs. knowledge bank relationship

See `00_Methodology/` for full statements.

---

## Knowledge Node Requirements

Every knowledge node SHOULD contain the metadata and sections defined in VRI-STR-006 and the template at `resources/node_template.md`.

**Linking Rules** (summary)
- One upstream authority
- One downstream operational artifact
- At least three related nodes
- Information exists once; other pages reference it

---

## Content Flywheel

Every completed research session SHOULD generate as many of the following as applicable:

- Reg Bible update
- Reg & Pol Notebook
- Context Map
- Action Map
- Playbook update
- FAQ
- Glossary entry
- Penumbrant Paper
- Client Advisory
- Newsletter content
- AI Knowledge Node

Never perform research for only one deliverable.

---

## Relationship to Public Product Site

The public-facing product site remains at:  
https://clearlinekris.github.io/CLRegMatrix/

That site is the simple, curated face.  
This repository is the deeper institutional knowledge bank.

Rules governing the relationship, linking, and projection are in **VRI-STR-010**.  
Templates live in `resources/`.  
A starter GitHub Actions workflow (`.github/workflows/project-to-public.yml`) can list nodes marked `public_status: ready` and open tracking issues/PRs in CLRegMatrix.

---

## Contribution Expectations

1. Prefer explanatory, practical, evidence-based, neutral, heavily cross-referenced writing.
2. Avoid marketing language, unnecessary legalese, unsupported conclusions.
3. Every directory MUST contain a README explaining purpose, contents, relationships, and contribution expectations.
4. Names describe concepts, not projects or version numbers.
5. Strengthen the shared body of institutional knowledge with every contribution.
6. Public projections must carry a clear Source of truth link back to this bank.

---

*Veridion · The clear line between regulation and relief.*  
© 2026
