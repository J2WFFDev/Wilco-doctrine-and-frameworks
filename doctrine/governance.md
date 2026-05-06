---
title: "Wilco Shooting Sports — Governance"
document_type: "doctrine"
status: "draft"
version: "0.1"
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
| `0.x` | Draft — content is incomplete or under active revision |
| `1.0` | First approved version — reviewed and accepted by Coach Jim West |
| `1.x` | Minor approved revision — section-level changes, additions |
| `x.0` | Major approved revision — structural or substantive overhaul |

### Version Increment Rules
- Increment the minor version (`0.1 → 0.2`) for any content change while in `draft` status.
- Increment to `1.0` when the document completes first formal review.
- Increment the minor version (`1.0 → 1.1`) for non-breaking updates after approval.
- Increment the major version (`1.x → 2.0`) for significant structural changes after approval.

---

## Status Values

| Status | Meaning |
|--------|---------|
| `draft` | Active working draft, subject to change |
| `in-review` | Submitted for review, pending approval |
| `approved` | Formally reviewed and accepted |
| `archived` | No longer active; kept for historical reference |

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

---

*Wilco Shooting Sports · Governance v0.1 · Draft*
