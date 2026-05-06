# Contributing to Wilco Shooting Sports Documentation

Thank you for contributing. This document explains the rules, conventions, and workflow that keep the repository consistent and trustworthy.

---

## Quick Reference

| What you want to do | How |
|---------------------|-----|
| Fix a typo or broken link | Commit directly to `main` |
| Add or update content in an existing file | Branch → PR → review |
| Create a new document | Branch → use a template → PR → review |
| Rename or move a file | Branch → PR → update all internal links |
| Change a term definition | Branch → update `doctrine/terminology.md` → PR → review |
| Propose a structural change | Open an issue first |

---

## Document Ownership and Approval

| Document Level | Who Can Edit | Final Approver |
|----------------|-------------|----------------|
| Doctrine | Any contributor (via PR) | Coach Jim West |
| Frameworks | Any contributor (via PR) | Program coach |
| Guides | Any contributor (via PR) | Program coach |
| Drills / Operations | Any contributor (via PR) | Any coach |
| Templates | Any contributor (via PR) | Any coach |

No document advances from `status: in-review` to `status: approved` without the named approver signing off on the PR.

---

## File and Folder Conventions

- **Filenames:** lowercase kebab-case, `.md` extension (e.g., `steel-performance-framework.md`)
- **Folders:** lowercase, no spaces (e.g., `doctrine/`, `frameworks/`)
- **One topic per file** — do not combine unrelated content
- **No duplicate definitions** — all terms live in `doctrine/terminology.md`

---

## Required Frontmatter

Every Markdown file must begin with YAML frontmatter. Use the appropriate template from `templates/`:

```yaml
---
title: "Exact Document Title"
document_type: "doctrine"          # doctrine | framework | guide | drill | operation | template
status: "draft"                    # draft | in-review | approved | archived
version: "0.1"
last_updated: "YYYY-MM-DD"
author: "Author Name"
organization: "Wilco Shooting Sports"
audience:
  - coaches                        # coaches | athletes | parents | volunteers | all
summary: "One-sentence summary."
related_documents:
  - "doctrine/terminology.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - draft
---
```

When you update a document, increment `version` and update `last_updated`.

---

## Terminology Control

**Rule:** All program terms are defined once in [`doctrine/terminology.md`](doctrine/terminology.md).

- Do **not** define a term in your document — link to `terminology.md` instead
- If a term is missing, add it to `terminology.md` in the same PR
- If a definition seems wrong, open an issue before changing it

---

## Status Lifecycle

```
draft → in-review → approved → archived
```

| Status | Meaning | Who Sets It |
|--------|---------|-------------|
| `draft` | Active work in progress | Author |
| `in-review` | Ready for review | Author (via PR) |
| `approved` | Reviewed and accepted | Approver |
| `archived` | No longer active | Approver |

---

## Branch and PR Conventions

- Branch name format: `docs/<short-description>` (e.g., `docs/update-terminology`, `docs/add-drill-draw-to-shot`)
- PR description should explain:
  - What changed and why
  - Which documents are affected
  - Whether any links were updated
- Request review from at least one other contributor
- Keep PRs focused — one topic per PR

---

## Document Hierarchy

When content in two documents conflicts, the higher level wins:

```
Level 1: doctrine/        ← Always wins
Level 2: frameworks/
Level 3: guides/
Level 4: drills/, operations/
Level 5: templates/, assets/
```

Flag conflicts by opening an issue, then resolve by updating the lower-level document.

---

## Internal Linking

Always use relative paths for internal links:

```markdown
See [terminology](doctrine/terminology.md#trigger-prep) for the definition.
See the [steel framework](../frameworks/steel-performance-framework.md).
```

When you rename or move a file, search for all references to it and update them in the same commit.

---

## Templates

Start every new document from the appropriate template in `templates/`:

| Document Type | Template |
|---------------|---------|
| Doctrine | `templates/doctrine-template.md` |
| Framework | `templates/framework-template.md` |
| Guide | `templates/guide-template.md` |
| Drill catalog | `templates/drill-template.md` |
| Operations | `templates/operation-template.md` |

---

## Review Cadence

| Level | Minimum Frequency |
|-------|------------------|
| Doctrine | Annually (or after major program change) |
| Frameworks | Annually (or after a season) |
| Guides | Annually (or when roles change) |
| Drills | As needed |
| Operations | Before each competitive season |

---

## Reference Documents

- [`README.md`](README.md) — repository overview and map
- [`doctrine/governance.md`](doctrine/governance.md) — versioning, hierarchy, approval rules, and GitHub editorial workflow
- [`doctrine/terminology.md`](doctrine/terminology.md) — all canonical term definitions
- [`docs/document-crosswalk.md`](docs/document-crosswalk.md) — concept map showing where topics live
- [`docs/docs-architecture.md`](docs/docs-architecture.md) — 3-tier architecture and Why vs. How separation
- [`docs/ai-workflow.md`](docs/ai-workflow.md) — rules for using ChatGPT and GitHub Copilot in this repository

---

*Wilco Shooting Sports · Contributing Guide · 2026-05-06*
