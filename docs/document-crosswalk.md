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
| **Serial vs. parallel execution model** | `frameworks/execution-models.md` | `frameworks/steel-performance-framework.md`, `drills/steel-drill-catalog.md` | Do not describe in drill notes |
| **Cognitive vs. mechanical overlap; compressed timing** | `frameworks/execution-models.md` | `guides/coach-guide.md` | Steel framework links; coach guide links |
| **Impact assessment taxonomy (visual/audible/predictive/index-feel/hybrid)** | `frameworks/impact-assessment-model.md` | `frameworks/steel-performance-framework.md`, `doctrine/terminology.md` (summary definition) | Do not collapse to "shot calling" — these are distinct concepts |
| **Match/Stage/String preparation layering** | `frameworks/preparation-framework.md` | `doctrine/master-doctrine.md` (summary), `guides/athlete-handbook.md` | Athlete handbook describes athlete behavior; prep-framework owns the model |
| **Visualization, VR, airgun, dry-fire tools** | `frameworks/preparation-framework.md` | `guides/athlete-handbook.md`, `guides/coach-guide.md` | Athlete handbook links, does not define |
| Precision/Bullseye execution model | `frameworks/precision-performance-framework.md` *(stub)* | `drills/precision-drill-catalog.md` *(stub)* | TBD |
| Data collection and metrics reporting | `frameworks/analytics-framework.md` *(stub)* | All frameworks | TBD |
| **Archery performance model** | `frameworks/archery-performance-framework.md` *(reserved)* | TBD — when program initiated | Reserved — do not add content until program is formally established |
| **Shotgun performance model** | `frameworks/shotgun-performance-framework.md` *(reserved)* | TBD — when program initiated | Reserved — do not add content until program is formally established |

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
| **Head Coach program leadership** | `guides/head-coach-guide.md` | `guides/coach-guide.md`, `guides/match-coach-guide.md` | Coach guide owns day-to-day coaching; head coach guide owns program-level responsibilities |
| **Match Coach role (vs. Practice and Head Coach)** | `guides/match-coach-guide.md` | `guides/head-coach-guide.md`, `frameworks/preparation-framework.md` | Match coaching is execution support — not technique development |
| **RSO role, qualifications, and authority** | `guides/range-safety-officer-guide.md` | `operations/match-operations.md`, `operations/range-safety-plan.md` | Match operations owns procedures; RSO guide owns the role and authority |
| **Scorekeeper role and data accuracy** | `guides/scorekeeper-guide.md` | `operations/match-operations.md`, `operations/match-director-guide.md` | Match score technician (data systems) is distinct from scorekeeper (field recorder) |
| **Sponsor relationships and tiers** | `guides/sponsor-guide.md` | `CREDITS.md` | One location for sponsor policies |
| **Visitors guide (first-time guests)** | `guides/visitors-guide.md` | `guides/new-shooter-orientation.md` | Visitors guide is for observers; orientation is for incoming athletes/families |
| **New shooter orientation** | `guides/new-shooter-orientation.md` | `guides/athlete-handbook.md`, `guides/parent-guide.md` | Orientation is the entry point; handbooks are the ongoing reference |

---

## Operations

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| The four fundamental safety rules | `doctrine/master-doctrine.md` (summary) + `operations/safety-manual.md` (full) | `guides/volunteer-guide.md`, `operations/range-operations.md` | Do not add a third copy in guides |
| Cease fire procedures | `operations/safety-manual.md` | `guides/volunteer-guide.md` | Guide should link, not restate |
| Safety violation policy | `operations/safety-manual.md` | `doctrine/master-doctrine.md` (summary only) | Safety manual owns the policy |
| Emergency procedures | `operations/safety-manual.md` | `operations/range-safety-plan.md` (site-specific application) | Safety manual owns policy; range safety plan owns site-specific steps |
| **Site-specific range safety (layout, roles, emergency steps)** | `operations/range-safety-plan.md` | `operations/safety-manual.md`, `guides/range-safety-officer-guide.md` | Safety manual is the policy; range safety plan is the site-specific application |
| Match-day coordinator checklist | `operations/match-operations.md` | `guides/volunteer-guide.md` | Volunteer guide describes roles; match-operations.md owns the checklist |
| Range commands | `operations/match-operations.md` | `guides/volunteer-guide.md`, `guides/range-safety-officer-guide.md` | Match-operations.md is the source; guides link |
| Range setup / teardown | `operations/range-operations.md` | `operations/match-operations.md` (match-specific subset) | Range-operations.md is the broader source |
| **Program equipment and supply tracking** | `operations/inventory-management.md` | `operations/range-operations.md` | One inventory system — do not maintain parallel lists |
| **Match Director and AMD authority** | `operations/match-director-guide.md` | `operations/match-operations.md`, `operations/event-management.md` | Match operations owns checklists; match director guide owns roles and authority |
| **Match committees (Range Prep, Startup, Awards, Teardown)** | `operations/match-director-guide.md` | `operations/event-management.md` | Match director guide owns committee structure |
| **Score arbitration and rules interpretation** | `operations/match-director-guide.md` | `guides/scorekeeper-guide.md` | Scorekeeper owns field data; match director guide owns dispute resolution |
| **Match Score Technician role** | `operations/match-director-guide.md` | `guides/scorekeeper-guide.md` | Distinct roles — do not collapse |
| **Event type catalog and operational profiles** | `operations/event-management.md` | All operations documents | Event management owns the event type taxonomy |
| **Squad assembly and competitor assignment** | `operations/match-organizer.md` | `operations/match-operations.md`, `operations/match-director-guide.md` | Match organizer owns squad assembly; match director owns match authority |

---

## Governance

| Topic | Canonical Home | Also Referenced In | Watch For Drift |
|-------|---------------|-------------------|----------------|
| Document hierarchy | `doctrine/governance.md` | `README.md`, `CONTRIBUTING.md` | README and CONTRIBUTING should summarize and link |
| Versioning rules | `doctrine/governance.md` | `CONTRIBUTING.md` | CONTRIBUTING should summarize and link |
| Status lifecycle | `doctrine/governance.md` | `README.md`, `CONTRIBUTING.md` | Consistent across all three |
| **GitHub editorial workflow (draft → approved)** | `doctrine/governance.md` | `CONTRIBUTING.md` | CONTRIBUTING summarizes steps; governance owns the policy |
| **3-tier documentation architecture** | `docs/docs-architecture.md` | `doctrine/governance.md`, `README.md` | README summarizes; docs-architecture.md owns the model |
| **Why vs. How separation** | `docs/docs-architecture.md` | `doctrine/governance.md`, `CONTRIBUTING.md` | Do not restate in every document — link |
| Contribution workflow | `CONTRIBUTING.md` | `README.md` | README summarizes; CONTRIBUTING is the source |
| Document ownership and approval | `CONTRIBUTING.md` | `doctrine/governance.md` | Governance is the policy; CONTRIBUTING is the how-to |
| **AI tool usage and governance** | `docs/ai-workflow.md` | `CONTRIBUTING.md` (brief reference) | One location only |

---

## Planned Content (Not Yet Written)

These topics are mentioned in existing documents but have no canonical home yet:

| Topic | Expected Canonical Home | Notes |
|-------|------------------------|-------|
| OGSM planning (program level) | `frameworks/analytics-framework.md` | Referenced in terminology |
| Session log template / format | `templates/shooter-performance-log.md` *(stub exists)* | Template created — expand with coaching examples |
| Coach feedback examples and journal prompts | `templates/shooter-performance-log.md` | Stub section exists |
| Seasonal planning process | `doctrine/governance.md` or `guides/coach-guide.md` | TBD |
| Precision execution model | `frameworks/precision-performance-framework.md` | Stub only |
| Group analysis methodology | `frameworks/precision-performance-framework.md` | Stub only |
| Athlete goal-setting worksheet | `guides/athlete-handbook.md` or `templates/` | OKR process described but no form exists |
| PARR model expanded (systems thinking, reflection timing, refinement culture) | `doctrine/master-doctrine.md` or new `doctrine/parr-model.md` | Currently a section; should be expanded |
| Mental performance (reflection timing, emotional recovery, confidence collapse) | `doctrine/philosophy.md` or new `frameworks/mental-performance.md` | Currently surface-level only |
| Metrics philosophy (metrics serving development, not replacing sportsmanship) | `frameworks/analytics-framework.md` | Covered in master-doctrine; needs its own section in analytics |
| AI workflow prompt templates | `docs/ai-workflow.md` | Stub section exists |
| Sponsor impact report template | `guides/sponsor-guide.md` or `templates/` | Referenced in sponsor guide |
| New shooter orientation presentation | `assets/presentations/` | Referenced in new-shooter-orientation.md |
| Incident report form | `operations/safety-manual.md` or `templates/` | Referenced in range-safety-plan.md |
| Score dispute form | `operations/match-director-guide.md` or `templates/` | Referenced in match director guide |
| Squad assignment tool / template | `operations/match-organizer.md` or `templates/` | Referenced in match organizer |
| Inventory master list (spreadsheet) | `assets/inventory/inventory-master.xlsx` | Referenced in inventory management |
| Diagram: PARR loop | `assets/diagrams/` | Not yet created |
| Diagram: Serial vs. parallel execution | `assets/diagrams/` | Not yet created |
| Diagram: Documentation hierarchy | `assets/diagrams/` | Not yet created |
| Diagram: Athlete development pathway | `assets/diagrams/` | Not yet created |
| Diagram: Preparation layers | `assets/diagrams/` | Not yet created |
| Diagram: Range layout | `assets/diagrams/range-layout.pdf` | Referenced in range-safety-plan.md |

---

*Wilco Shooting Sports · Document Crosswalk v0.1 · Draft*
