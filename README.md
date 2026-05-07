# Wilco Shooting Sports — Doctrine & Frameworks Repository

## 1. Repository Purpose

This repository is the authoritative source for all doctrine, frameworks, guides, drill catalogs, and operational documents for **Wilco Shooting Sports**. It exists to give coaches, athletes, parents, and volunteers a consistent, versioned reference for how we train, compete, and operate.

---

## 2. Collaboration Intent

This repo is a living working draft. All contributors are encouraged to:

- Open **issues** for significant document tasks, questions, or flags
- Use **branches** for larger rewrites or new sections
- Submit **pull requests** for structural or content changes
- Keep documents in `status: draft` until formally reviewed

---

## 3. Document Hierarchy

```
doctrine/        ← Core beliefs, values, and governance rules
frameworks/      ← Structured performance and execution systems
guides/          ← Role-specific handbooks (athlete, parent, coach, volunteer)
drills/          ← Drill catalogs organized by program (Steel, Precision)
operations/      ← Match operations, safety, and range procedures
assets/          ← Diagrams, logos, graphics
templates/       ← Starter templates for new documents and drills
```

**Precedence:** Doctrine → Frameworks → Guides → Drills / Operations

When conflicts exist between documents, the document higher in the hierarchy takes precedence. Flag conflicts with an issue.

---

## 4. Writing Conventions

- **Filenames:** lowercase kebab-case (`master-doctrine.md`, `steel-performance-framework.md`)
- **Headings:** Title Case for H1 and H2; sentence case for H3 and below
- **Terminology:** Use definitions from `doctrine/terminology.md` — do not redefine terms locally
- **Cross-references:** Link to the relevant file using relative paths (e.g., `[terminology](doctrine/terminology.md)`)
- **Status:** Every document must carry a `status` frontmatter field

---

## 5. Frontmatter Standard

Every main document must begin with YAML frontmatter:

```yaml
---
title: "Document Title"
document_type: "doctrine"         # doctrine | framework | guide | drill | operation | template
status: "draft"                   # draft | in-review | approved | archived
version: "0.1"
last_updated: "YYYY-MM-DD"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches                       # coaches | athletes | parents | volunteers | all
summary: "Short summary."
related_documents:
  - "doctrine/terminology.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - doctrine
  - draft
---
```

### Status Values

| Status | Meaning |
|--------|---------|
| `draft` | Active working draft, subject to change |
| `in-review` | Submitted for review, pending approval |
| `approved` | Formally reviewed and accepted |
| `archived` | No longer active; kept for reference |

---

## 6. Terminology Standard

All standardized terms are defined in [`doctrine/terminology.md`](doctrine/terminology.md).

**Rule:** Other documents reference that file — they do not redefine terms. If a term is missing, open an issue or add it to `terminology.md` directly.

---

## 7. Contribution Workflow

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for the full contribution guide, including document ownership, approval workflow, branch conventions, and terminology control.

Quick summary:

1. **Open an issue** describing what you want to add or change
2. **Create a branch** from `main` (e.g., `docs/update-terminology`)
3. **Make your changes** using the appropriate template from `templates/`
4. **Submit a pull request** to `main` with a clear description
5. **Request review** from at least one other contributor

For small fixes (typos, formatting), you may commit directly to `main`.

---

## 8. Repository Map

```
README.md                              ← This file
CONTRIBUTING.md                        ← Contribution rules, ownership, workflow
CREDITS.md                             ← Authors, contributors, and organizational attribution
docs/
  document-crosswalk.md                ← Concept map: where each topic lives canonically
  docs-architecture.md                 ← 3-tier architecture and Why vs. How separation
  ai-workflow.md                       ← Rules for using ChatGPT and Copilot in this repo
doctrine/
  master-doctrine.md                   ← Purpose, mission, vision, values, development model
  terminology.md                       ← Canonical definitions for all program terms
  philosophy.md                        ← Coaching, competition, and youth development philosophy
  governance.md                        ← Document hierarchy, versioning, GitHub editorial workflow
frameworks/
  steel-performance-framework.md       ← SASP execution model and performance system
  precision-performance-framework.md   ← Precision/NRA Bullseye performance framework (stub)
  execution-models.md                  ← Serial vs. parallel execution; cognitive/mechanical overlap
  impact-assessment-model.md           ← Visual, audible, predictive, index/feel, hybrid assessment
  preparation-framework.md             ← Match, stage, and string preparation layering
  analytics-framework.md               ← Data collection, metrics, and reporting (stub)
  archery-performance-framework.md     ← Archery framework (reserved — not yet active)
  shotgun-performance-framework.md     ← Shotgun framework (reserved — not yet active)
guides/
  athlete-handbook.md                  ← Athlete expectations, routines, and competition prep
  parent-guide.md                      ← Parent roles, expectations, and team culture
  coach-guide.md                       ← Day-to-day coaching practices, planning, and communication
  head-coach-guide.md                  ← Head Coach program leadership and coach development
  match-coach-guide.md                 ← Match-day athlete support; distinct from practice coaching
  volunteer-guide.md                   ← Volunteer roles, setup, and range safety responsibilities
  range-safety-officer-guide.md        ← RSO role, qualifications, authority, and procedures
  scorekeeper-guide.md                 ← Scorekeeper role, data accuracy, and dispute escalation
  sponsor-guide.md                     ← Sponsor tiers, expectations, and relationship management
  visitors-guide.md                    ← First-time visitors and prospective families
  new-shooter-orientation.md           ← New athlete onboarding: safety, expectations, first sessions
drills/
  steel-drill-catalog.md               ← Drill library for SASP training
  precision-drill-catalog.md           ← Drill library for Precision/Bullseye training (stub)
operations/
  match-operations.md                  ← Match-day checklists and Range Officer procedures
  match-director-guide.md              ← Match Director, AMD, committees, rules, score technician
  match-organizer.md                   ← Squad assembly and competitor assignment
  event-management.md                  ← Event type catalog and operational profiles
  safety-manual.md                     ← Range safety rules, emergency procedures, protocols
  range-safety-plan.md                 ← Site-specific range safety: layout, roles, emergency steps
  range-operations.md                  ← Range setup, teardown, and daily operations
  inventory-management.md              ← Program equipment and supply tracking
assets/
  diagrams/                            ← Diagrams and charts
  logos/                               ← Organization logos and marks
  graphics/                            ← Supporting graphics and visual aids
  presentations/                       ← Presentation decks (new shooter orientation, etc.)
  inventory/                           ← Inventory master list and asset records
templates/
  document-template.md                 ← Generic starter template
  doctrine-template.md                 ← Doctrine-specific starter
  framework-template.md                ← Framework-specific starter
  guide-template.md                    ← Guide-specific starter
  drill-template.md                    ← Drill entry starter
  operation-template.md                ← Operations document starter
  shooter-performance-log.md           ← Session/match performance data, journal, and coach feedback
```

---

*Wilco Shooting Sports · Maintained by Coach Jim West · All documents subject to revision*
