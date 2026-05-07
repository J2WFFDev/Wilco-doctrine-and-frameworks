---
title: "Documentation Architecture"
document_type: "doctrine"
status: "draft"
version: "0.1"
last_updated: "2026-05-06"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches
summary: "Defines the 3-tier documentation architecture, the Why vs How separation, and the rules governing how document types relate to each other. This is the architectural blueprint for the entire knowledge system."
related_documents:
  - "doctrine/governance.md"
  - "doctrine/master-doctrine.md"
  - "docs/document-crosswalk.md"
  - "CONTRIBUTING.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - architecture
  - governance
  - draft
---

# Documentation Architecture

> This document defines **how** the knowledge system is structured and **why** each tier exists. It is the architectural blueprint that prevents document chaos as the repository grows.

---

## The 3-Tier Document Architecture

All documents in this repository belong to one of three tiers. Each tier has a distinct purpose and a different rate of change.

| Tier | Folder(s) | Purpose | Change Rate |
|------|-----------|---------|-------------|
| **Tier 1 — Doctrine** | `doctrine/` | Stable philosophy, values, definitions, governance | Slow — annually or on major program change |
| **Tier 2 — Frameworks & Guides** | `frameworks/`, `guides/` | Technical systems, role expectations, structured methods | Moderate — seasonally or on program evolution |
| **Tier 3 — Operational Artifacts** | `drills/`, `operations/` | Procedures, catalogs, checklists, how-to references | Fast — as needed, before each season |

### Tier 1 — Doctrine

Doctrine is the most stable layer. It answers **WHY**.

- Why this program exists
- Why we train the way we train
- Why character matters as much as performance
- Why we use the terminology we use
- Why documents are structured the way they are

Doctrine documents should rarely need updating. If content changes frequently, it probably belongs in a lower tier.

**Doctrine files:**
- [`master-doctrine.md`](../doctrine/master-doctrine.md) — Mission, vision, values, development model
- [`philosophy.md`](../doctrine/philosophy.md) — Coaching, competition, youth development, family philosophy
- [`terminology.md`](../doctrine/terminology.md) — Canonical definitions for all program terms
- [`governance.md`](../doctrine/governance.md) — Document hierarchy, versioning, approval process
- This file — Documentation architecture

---

### Tier 2 — Frameworks & Guides

Frameworks and Guides operationalize doctrine. They answer **HOW** and **WHAT**.

- Frameworks describe **HOW** we train, measure, and develop athletes
- Guides describe **WHAT** each role does

These documents should be consistent with doctrine. If a framework contradicts doctrine, the framework is wrong.

**Framework files:**
- [`steel-performance-framework.md`](../frameworks/steel-performance-framework.md) — SASP execution model and performance system
- [`precision-performance-framework.md`](../frameworks/precision-performance-framework.md) — Precision/NRA Bullseye performance framework
- [`execution-models.md`](../frameworks/execution-models.md) — Serial vs. parallel execution, cognitive vs. mechanical overlap
- [`impact-assessment-model.md`](../frameworks/impact-assessment-model.md) — Visual, audible, predictive, and hybrid impact assessment taxonomy
- [`preparation-framework.md`](../frameworks/preparation-framework.md) — Match, stage, and string preparation layering
- [`analytics-framework.md`](../frameworks/analytics-framework.md) — Data collection, metrics, and reporting

**Guide files:**
- [`athlete-handbook.md`](../guides/athlete-handbook.md) — Athlete expectations, routines, competition prep
- [`coach-guide.md`](../guides/coach-guide.md) — Coaching practices, planning, feedback model
- [`parent-guide.md`](../guides/parent-guide.md) — Parent roles, expectations, team culture
- [`volunteer-guide.md`](../guides/volunteer-guide.md) — Volunteer roles, setup, safety responsibilities

---

### Tier 3 — Operational Artifacts

Operational documents are the most practical and most frequently updated tier. They answer **WHEN** and **HOW specifically**.

- Checklists, catalogs, and procedures
- Content that changes with seasons, venues, or rosters

**Operational files:**
- [`steel-drill-catalog.md`](../drills/steel-drill-catalog.md) — Drill library for SASP
- [`precision-drill-catalog.md`](../drills/precision-drill-catalog.md) — Drill library for Precision/Bullseye
- [`match-operations.md`](../operations/match-operations.md) — Match-day procedures and checklists
- [`safety-manual.md`](../operations/safety-manual.md) — Range safety rules, emergency procedures
- [`range-operations.md`](../operations/range-operations.md) — Range setup, teardown, daily operations

---

## The Why vs. How Separation

This distinction is the single most important architectural principle.

| Document Type | Question It Answers | Example |
|---------------|---------------------|---------|
| **Doctrine** | WHY | "Why do we prioritize process over score?" |
| **Framework** | HOW | "How do we classify and review a stage run?" |
| **Guide** | WHAT (role-specific) | "What does a coach do during a post-match debrief?" |
| **Drill/Operation** | WHEN / HOW SPECIFICALLY | "When does the RO issue the 'Make Ready' command?" |

**Rule:** If you find yourself asking "why?" and the answer isn't in a doctrine document, the doctrine is incomplete. If you find yourself asking "how?" and the answer is in a doctrine document, the content may be misplaced.

---

## Precedence Rules

When documents conflict, the higher tier wins:

```
Doctrine  >  Frameworks  >  Guides  >  Drills / Operations
```

This means:
- A guide may not contradict a framework
- A framework may not contradict doctrine
- Operational procedures may not contradict guides

When you find a conflict, flag it with a GitHub issue. Resolve it by updating the lower-tier document to align with the higher-tier one — never by weakening the higher-tier document.

---

## Navigation Guide

Not sure where to put something? Use this decision tree:

1. **Is it a definition, value, or architectural rule?** → `doctrine/`
2. **Is it a structured performance or training system?** → `frameworks/`
3. **Is it role-specific guidance (what someone should do)?** → `guides/`
4. **Is it a drill, checklist, or operational procedure?** → `drills/` or `operations/`
5. **Is it reusable as a starting template?** → `templates/`
6. **Is it a visual, diagram, or graphic?** → `assets/`

When in doubt, check [`docs/document-crosswalk.md`](document-crosswalk.md) — it shows the canonical home for every major topic.

---

## Diagram: Architecture Overview

```
┌─────────────────────────────────────────────────┐
│  TIER 1 — DOCTRINE  (doctrine/)                 │
│  WHY  ·  stable  ·  slow-changing               │
│  master-doctrine · philosophy · terminology      │
│  governance · docs-architecture                  │
└────────────────────┬────────────────────────────┘
                     │ derived from
┌────────────────────▼────────────────────────────┐
│  TIER 2 — FRAMEWORKS & GUIDES                   │
│  (frameworks/ · guides/)                        │
│  HOW / WHAT  ·  moderate change                 │
│  steel-framework · execution-models             │
│  impact-assessment · preparation-framework      │
│  athlete-handbook · coach-guide · parent-guide  │
└────────────────────┬────────────────────────────┘
                     │ derived from
┌────────────────────▼────────────────────────────┐
│  TIER 3 — OPERATIONAL ARTIFACTS                 │
│  (drills/ · operations/)                        │
│  WHEN / HOW SPECIFICALLY  ·  fast-changing      │
│  drill-catalogs · match-ops · safety-manual     │
└─────────────────────────────────────────────────┘
```

---

*Wilco Shooting Sports · Documentation Architecture v0.1 · Draft*
