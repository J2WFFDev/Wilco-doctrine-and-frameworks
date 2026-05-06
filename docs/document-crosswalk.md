---
title: "Document Crosswalk"
document_type: "doctrine"
status: "draft"
version: "0.1"
last_updated: "2026-05-06"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches
summary: "A concept map showing where each major topic lives canonically, where it is referenced across the repository, and where documents should cross-link."
related_documents:
  - "doctrine/master-doctrine.md"
  - "doctrine/governance.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - governance
  - crosswalk
  - draft
---

# Document Crosswalk

This file is the concept map for the Wilco Shooting Sports documentation repository. It shows where each major topic **lives canonically**, where it is **referenced**, and where **potential overlap** should be monitored.

Use this when:
- Deciding where to put new content
- Checking whether something already exists before writing it
- Reviewing a PR that touches shared concepts

---

## How to Read This Table

| Column | Meaning |
|--------|---------|
| **Topic** | A major concept or content area |
| **Canonical Home** | The file that owns the authoritative definition or content |
| **Also Referenced In** | Files that link to or use this content |
| **Watch For Drift** | Files that might accidentally duplicate this content |

---

## Core Doctrine

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Mission, Vision, Values | `doctrine/master-doctrine.md` | `README.md`, `guides/athlete-handbook.md` | All guides |
| Athlete Development Stages (Foundation / Development / Performance) | `doctrine/master-doctrine.md` | `guides/coach-guide.md`, `drills/steel-drill-catalog.md` | Frameworks |
| Coaching Philosophy | `doctrine/philosophy.md` | `doctrine/master-doctrine.md` (summary), `guides/coach-guide.md` | Guide content |
| Competition Philosophy | `doctrine/philosophy.md` | `guides/athlete-handbook.md` | Coach guide |
| Youth Development Philosophy | `doctrine/philosophy.md` | `guides/parent-guide.md`, `guides/athlete-handbook.md` | All guides |
| Family Support Philosophy | `doctrine/philosophy.md` | `guides/parent-guide.md` | Parent guide |
| Sportsmanship and Leadership | `doctrine/philosophy.md` | `guides/athlete-handbook.md`, `guides/volunteer-guide.md` | All guides |
| Safety Doctrine (core rules) | `doctrine/master-doctrine.md` | `operations/safety-manual.md` (full), `guides/volunteer-guide.md` | Do not duplicate full rules outside safety-manual.md |
| Reflection Model (Observe–Assess–Decide–Act) | `doctrine/master-doctrine.md` | `guides/coach-guide.md`, `guides/athlete-handbook.md` | Separate from PARR — note distinction |

---

## Terminology

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| All program terms (full list) | `doctrine/terminology.md` | Every document via link | Every document — link, do not define locally |
| Impact Assessment | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md` | Drill catalog notes |
| Shot Calling | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md` | Guide content |
| Trigger Prep / Reset | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md` | Drill notes |
| Shot Break | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md` | Drill notes |
| Predictive vs. Confirmed Execution | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md` | Do not redefine in drill notes |
| Transition Efficiency | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md` | Drill catalog |
| Presentation | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md` | Drill notes |
| Clean / Sloppy / Recovery Run | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md`, `guides/coach-guide.md` | All coaching content |
| Stage Preparation / String Preparation | `doctrine/terminology.md` | `guides/athlete-handbook.md`, `operations/match-operations.md` | Handbooks |
| PARR | `doctrine/terminology.md` | `doctrine/master-doctrine.md` (Reflection Model adjacent), `guides/athlete-handbook.md`, `guides/coach-guide.md`, `drills/steel-drill-catalog.md` | Note distinction from Observe–Assess–Decide–Act |
| OKR | `doctrine/terminology.md` | `guides/athlete-handbook.md`, `guides/coach-guide.md` | Seasonal planning docs |
| OGSM | `doctrine/terminology.md` | Program-level planning (not yet in a file) | Analytics framework when developed |
| Bio-Condition | `doctrine/terminology.md` | `frameworks/steel-performance-framework.md`, `frameworks/analytics-framework.md` | Session log templates |

---

## Performance Frameworks

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Steel Challenge execution model | `frameworks/steel-performance-framework.md` | `drills/steel-drill-catalog.md` | Do not describe execution model in the drill catalog |
| Run classification system | `frameworks/steel-performance-framework.md` + definitions in `doctrine/terminology.md` | `guides/coach-guide.md`, `drills/steel-drill-catalog.md` | Guides should link, not define |
| Performance components (Technical / Mental / Physical) | `frameworks/steel-performance-framework.md` | `guides/coach-guide.md`, `drills/steel-drill-catalog.md` | Do not duplicate component definitions in drill notes |
| Metrics hierarchy (Tiers 1–6) | `frameworks/steel-performance-framework.md` | `frameworks/analytics-framework.md` (when developed) | Analytics framework |
| Environment and bio-condition tracking | `frameworks/steel-performance-framework.md` | `frameworks/analytics-framework.md` (when developed) | Analytics framework |
| Equipment baseline tracking | `frameworks/steel-performance-framework.md` | `frameworks/analytics-framework.md` (when developed) | Coach guide |
| Precision/Bullseye execution model | `frameworks/precision-performance-framework.md` *(stub)* | `drills/precision-drill-catalog.md` *(stub)* | TBD |
| Data collection and metrics reporting | `frameworks/analytics-framework.md` *(stub)* | All frameworks | TBD |

---

## Drill Catalogs

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Drill structure/format | `templates/drill-template.md` | `drills/steel-drill-catalog.md`, `drills/precision-drill-catalog.md` | All drill files |
| Steel Challenge drills (library) | `drills/steel-drill-catalog.md` | `frameworks/steel-performance-framework.md` (references catalog) | Do not define drills in the framework |
| Performance standards per stage | `drills/steel-drill-catalog.md` | `guides/athlete-handbook.md` | Coach guide |
| Precision/Bullseye drills | `drills/precision-drill-catalog.md` *(stub)* | `frameworks/precision-performance-framework.md` | TBD |

---

## Guides

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Athlete expectations and routines | `guides/athlete-handbook.md` | `guides/parent-guide.md` (role boundary), `guides/coach-guide.md` | Do not duplicate in parent guide |
| Parent role and conduct | `guides/parent-guide.md` | `doctrine/philosophy.md` (philosophy section), `guides/athlete-handbook.md` | Parent guide owns the role definition |
| Coaching practices and feedback model | `guides/coach-guide.md` | `doctrine/philosophy.md` (philosophy), `doctrine/master-doctrine.md` (summary) | Philosophy.md owns the "why"; coach-guide.md owns the "how" |
| Volunteer roles and responsibilities | `guides/volunteer-guide.md` | `operations/match-operations.md` (RO procedures overlap) | Volunteer guide defines roles; operations owns procedures |

---

## Operations

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| The four fundamental safety rules | `doctrine/master-doctrine.md` (summary) + `operations/safety-manual.md` (full) | `guides/volunteer-guide.md`, `operations/range-operations.md` | Do not add a third copy in guides |
| Cease fire procedures | `operations/safety-manual.md` | `guides/volunteer-guide.md` | Guide should link, not restate |
| Safety violation policy | `operations/safety-manual.md` | `doctrine/master-doctrine.md` (summary only) | Safety manual owns the policy |
| Emergency procedures | `operations/safety-manual.md` | `operations/range-operations.md` (closing checklist reference) | One location only |
| Match-day coordinator checklist | `operations/match-operations.md` | `guides/volunteer-guide.md` | Volunteer guide describes roles; match-operations.md owns the checklist |
| Range commands | `operations/match-operations.md` | `guides/volunteer-guide.md` (RO section) | Match-operations.md is the source; volunteer guide links |
| Range setup / teardown | `operations/range-operations.md` | `operations/match-operations.md` (match-specific subset) | Range-operations.md is the broader source |
| Equipment inventory and maintenance log | `operations/range-operations.md` | | |

---

## Governance

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Document hierarchy | `doctrine/governance.md` | `README.md`, `CONTRIBUTING.md` | README and CONTRIBUTING should summarize and link |
| Versioning rules | `doctrine/governance.md` | `CONTRIBUTING.md` | CONTRIBUTING should summarize and link |
| Status lifecycle | `doctrine/governance.md` | `README.md`, `CONTRIBUTING.md` | Consistent across all three |
| Contribution workflow | `CONTRIBUTING.md` | `README.md` | README summarizes; CONTRIBUTING is the source |
| Document ownership and approval | `CONTRIBUTING.md` | `doctrine/governance.md` | Governance is the policy; CONTRIBUTING is the how-to |

---

## Planned Content (Not Yet Written)

These topics are mentioned in existing documents but have no canonical home yet:

| Topic | Expected Canonical Home | Notes |
|-------|------------------------|-------|
| OGSM planning (program level) | `frameworks/analytics-framework.md` | Referenced in terminology |
| Session log template / format | `frameworks/analytics-framework.md` or a `templates/` file | Bio-condition tracking referenced in frameworks |
| Seasonal planning process | `doctrine/governance.md` or `guides/coach-guide.md` | TBD |
| Precision execution model | `frameworks/precision-performance-framework.md` | Stub only |
| Group analysis methodology | `frameworks/precision-performance-framework.md` | Stub only |
| Athlete goal-setting worksheet | `guides/athlete-handbook.md` or `templates/` | OKR process described but no form exists |

---

*Wilco Shooting Sports · Document Crosswalk v0.1 · Draft*
