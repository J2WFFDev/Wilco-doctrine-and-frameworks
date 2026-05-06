---
title: "Wilco Shooting Sports — Governance"
document_type: "doctrine"
status: "draft"
version: "0.2"
last_updated: "2026-05-06"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches
summary: "Document governance rules including hierarchy, versioning, review cadence, contribution expectations, and the approval and revision process."
related_documents:
  - "doctrine/master-doctrine.md"
  - "doctrine/terminology.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - doctrine
  - governance
  - draft
---

# Wilco Shooting Sports — Governance

---

## Document Hierarchy

All documents in this repository exist within a defined hierarchy. Documents higher in the hierarchy take precedence when conflicts exist.

```
Level 1: Doctrine          (doctrine/)
Level 2: Frameworks        (frameworks/)
Level 3: Guides            (guides/)
Level 4: Drills/Operations (drills/, operations/)
Level 5: Templates/Assets  (templates/, assets/)
```

If a guide contradicts a framework, the framework wins. If a framework contradicts doctrine, doctrine wins. Conflicts should be flagged via a GitHub issue and resolved by updating the lower-level document.

---

## Document Types

| Type | Folder | Purpose |
|------|--------|---------|
| `doctrine` | `doctrine/` | Core beliefs, values, canonical definitions, governance |
| `framework` | `frameworks/` | Structured performance and execution systems |
| `guide` | `guides/` | Role-specific handbooks and expectations |
| `drill` | `drills/` | Drill catalogs and training prescriptions |
| `operation` | `operations/` | Match-day, safety, and range procedures |
| `template` | `templates/` | Starter templates for new documents |

---

## Versioning Rules

Every document carries a `version` field in its YAML frontmatter.

### Version Numbering

| Version Pattern | When to Use |
|-----------------|-------------|
| `0.0` | Placeholder — file scaffolded from template; no substantive content |
| `0.x` | Pre-approval — content in active development, draft, or in-review |
| `1.0` | First approved version — reviewed and accepted by Coach Jim West |
| `1.x` | Minor approved revision — section-level changes, additions |
| `x.0` | Major approved revision — structural or substantive overhaul |

### Version Increment Rules
- Set `0.0` when a file is first created from a template (`placeholder` status).
- Increment to `0.1` when substantive content development begins (`dev` status).
- Increment the minor version (`0.1 → 0.2`) for any content change during `dev` or `draft` status.
- Version numbers during `dev` and `draft` represent iteration (Draft 1 = `0.1`, Draft 2 = `0.2`, etc.).
- Increment to `1.0` when the document completes first formal review and is approved.
- Increment the minor version (`1.0 → 1.1`) for non-breaking updates after approval.
- Increment the major version (`1.x → 2.0`) for significant structural changes after approval.

---

## Status Values

| Status | Meaning | Version |
|--------|---------|---------|
| `placeholder` | File scaffolded — frontmatter and section headings only; no substantive content | `0.0` |
| `dev` | Active content development — rough, AI-assisted, or sections still incomplete | `0.1+` |
| `draft` | First complete, coherent document — whole thought is present and readable; ready for editorial review | `0.x` |
| `in-review` | Submitted for review via PR; pending approval | `0.x` |
| `approved` | Formally reviewed, accepted, and merged to `main` — the authoritative reference | `1.0+` |
| `archived` | No longer active; superseded or retired — kept for historical reference | unchanged |

> **Note on `planned`:** Documents that are identified as needed but do not yet exist as files are tracked as GitHub Issues with a `status: planned` label — not as files in the repository. A file is created only when development begins, starting at `placeholder`.

Documents must not be used as authoritative references until they reach `approved` status.

---

## Review Cadence

| Document Level | Minimum Review Frequency |
|----------------|--------------------------|
| Doctrine | Annually, or after significant program change |
| Frameworks | Annually, or after a competitive season |
| Guides | Annually, or when roles or expectations change |
| Drills | As needed; following new drill additions |
| Operations | Prior to each competitive season |

---

## Contribution Expectations

### All Contributors
- Follow the naming and frontmatter conventions in [README.md](../README.md).
- Reference [doctrine/terminology.md](terminology.md) for all program terms.
- Do not change another contributor's document without creating an issue first.
- Keep commits focused on a single change or document.

### Coaches
- Responsible for keeping their assigned documents current.
- Flag outdated or conflicting content via GitHub issues.
- Review pull requests from other contributors within 7 days when requested.

### Program Director (Coach Jim West)
- Final approver for all documents at Level 1 (Doctrine).
- Final approver for all status changes from `in-review` to `approved`.
- Responsible for resolving hierarchy conflicts.

---

## Approval and Revision Process

### New Document
1. Create file from `templates/document-template.md`
2. Set `status: draft`
3. Write content; increment version as changes accumulate
4. Open a pull request targeting `main` when ready for review
5. Request review; address feedback
6. Upon approval, update `status: in-review` → `approved`

### Revising an Existing Document
1. Create a branch (e.g., `docs/update-governance`)
2. Make changes; increment version
3. Update `last_updated` date
4. Open a pull request; describe what changed and why
5. Obtain review; update status as appropriate

### Emergency Correction (Typos / Safety Errors)
- Minor corrections (typos, broken links) may be committed directly to `main`.
- Safety-related corrections are treated as urgent and may bypass normal review timing, but must still be documented via a pull request.

---

## How Doctrine Relates to Other Document Types

```
doctrine/master-doctrine.md
  └── Establishes values and development model
        ├── frameworks/          ← Operationalize values into structured systems
        │     └── describe HOW we train and measure
        ├── guides/              ← Translate values into role-specific expectations
        │     └── describe WHAT each role does
        └── operations/          ← Apply values in procedural form
              └── describe WHEN and HOW operations are conducted
```

Frameworks, guides, and operations may not contradict doctrine. When drafting any document, check [master-doctrine.md](master-doctrine.md) and [terminology.md](terminology.md) first.

> For full architecture detail and the Why vs. How separation, see [docs/docs-architecture.md](../docs/docs-architecture.md).

---

## GitHub Editorial Workflow

This section explains how GitHub's native tools map to the document editorial process — from first draft through publication.

### The Core Concept

Git tracks every change to every file automatically. You never lose a version. The `status` field in frontmatter tells readers what state a document is in. Together, these two systems give you full editorial control without a separate document management tool.

```
Git history         ← Every change, forever, who made it and when
Frontmatter status  ← Where the document is in the editorial lifecycle
GitHub PRs          ← The editorial review and approval mechanism
GitHub Issues       ← The task and feedback tracking system
```

---

### Draft to Published: Step by Step

#### Step 1 — Open an Issue (Planned)

Before creating a new document or making a significant change, open a GitHub Issue describing:
- What document you are creating or changing
- Why it is needed
- Which other documents it affects

Apply the `status: planned` label. This creates a traceable record of intent and allows others to weigh in before work begins. The document does not exist as a file yet — that happens in Step 2.

#### Step 2 — Create a Branch

Create a new branch from `main` for your work:

```
docs/new-execution-models
docs/update-terminology-v02
docs/revise-steel-framework
```

Never write draft content directly on `main`. The `main` branch is the stable, clean reference version of the repository.

#### Step 3 — Write and Iterate

Create the file from the appropriate template in `templates/`. The file begins at `status: placeholder`, `version: 0.0`.

- When you begin adding substantive content, change `status` to `dev` and increment version to `0.1`.
- Continue incrementing version as content grows (`0.1 → 0.2 → 0.3`). Each version is a numbered draft iteration.
- When the document is a complete, coherent first pass — whole thought present, readable end-to-end — change `status` to `draft`.
- Commit frequently with descriptive commit messages.

#### Step 4 — Open a Pull Request

When the document reaches `draft` status and is ready for review, open a Pull Request (PR) targeting `main`. The PR description should explain:
- What changed and why
- Which documents are affected
- Whether any links were added or updated

Change the frontmatter `status` to `in-review` in this PR.

#### Step 5 — Review

One or more reviewers read the document and leave comments in the PR. The author addresses feedback and makes additional commits to the same branch. The PR conversation becomes the editorial record.

#### Step 6 — Approve and Merge

When the reviewer approves the PR:
1. Change `status: in-review` → `status: approved`
2. Set `version` to the first production number (`1.0` for first approval, `1.x` for subsequent)
3. Merge the PR into `main`

The document is now "published." The merge date is visible in Git history.

---

### Draft vs. Published Summary

| State | Frontmatter Status | Branch | Notes |
|-------|-------------------|--------|-------|
| Planned (no file yet) | — | Issues only | Tracked as a GitHub Issue with `status: planned` label |
| File created, headings only | `placeholder` | Feature branch | Not readable content |
| Active writing | `dev` | Feature branch | Rough, AI-assisted, incomplete sections |
| Complete first pass | `draft` | Feature branch | Whole thought present; ready for editorial review |
| Ready for review | `in-review` | Feature branch via PR | Under editorial review |
| **Published / Authoritative** | **`approved`** | **Merged to `main`** | **Authoritative reference** |
| Replaced | `archived` | On `main` | Kept for history |

**"Published" = `status: approved` on `main`.**

Readers who want only authoritative content should filter for `status: approved` documents. Documents at `placeholder`, `dev`, or `draft` status are working material, not final references.

> **How to see a document's history:** On GitHub, navigate to any file → click **History**. Every commit that changed that file is listed, with the exact content at each version. This is how you review prior drafts, compare versions, and trace the editorial record — no separate branch system is needed.

---

### Using GitHub Labels

Apply labels to Issues and PRs to communicate state at a glance:

| Label | Meaning |
|-------|---------|
| `status: planned` | Identified as needed; Issue open, no file yet |
| `status: placeholder` | File exists with headings only; no substantive content |
| `status: dev` | Active content development underway |
| `status: draft` | First complete readable pass; ready for editorial review |
| `status: in-review` | PR is open and awaiting review |
| `status: approved` | Merged; document is authoritative |
| `status: archived` | No longer active; retained for history |
| `type: doctrine` | Change affects doctrine-level content |
| `type: terminology` | Change affects `terminology.md` |
| `type: new-doc` | Creates a new document |
| `priority: high` | Needs attention before the next session or match |

---

### Using GitHub Releases for Repo Snapshots

GitHub Releases allow you to tag a specific snapshot of the entire repository as a named version — useful for "Season 2026 approved documents" or "Approved for print."

To create a release:
1. Go to the repository → Releases → Draft a new release
2. Tag it with a version (e.g., `v2026.1` or `season-2026`)
3. Describe which documents are approved and what this release represents

This gives you a permanent, downloadable snapshot of the entire repository at that point in time — useful for printing, sharing with families, or archiving before a major revision cycle.

---

### Quick Reference: GitHub Tools Map

| Situation | GitHub Tool |
|-----------|-------------|
| Track a planned document or known gap | Issue (label: `status: planned`) |
| Scaffold a new file from template | Create file; set `status: placeholder`, `version: 0.0` |
| Begin writing content | Set `status: dev`, increment to `0.1` |
| Document is complete first pass | Set `status: draft` |
| Propose content for review | Pull Request |
| Provide feedback on a document | PR review comments |
| Flag a conflict between two documents | Issue |
| Mark a document as authoritative | Merge PR; set `status: approved`, `version: 1.0` |
| Archive a replaced document | Set `status: archived` in a commit |
| See a document's prior drafts | GitHub → file → History |
| Snapshot the full repo for a season | GitHub Release |
| See who changed what and when | Git commit history |

---

*Wilco Shooting Sports · Governance v0.2 · Draft*
