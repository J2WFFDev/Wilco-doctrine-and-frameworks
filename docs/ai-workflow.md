---
title: "AI Workflow Guide"
document_type: "doctrine"
status: "draft"
version: "0.1"
last_updated: "2026-05-06"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches
summary: "Defines how AI tools (ChatGPT and GitHub Copilot) are used in this repository, what each tool is responsible for, what changes require human review, and how to preserve terminology and doctrine integrity when working with AI assistance."
related_documents:
  - "doctrine/governance.md"
  - "doctrine/terminology.md"
  - "CONTRIBUTING.md"
  - "docs/docs-architecture.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - governance
  - ai-workflow
  - draft
---

# AI Workflow Guide

> This guide exists because AI tools touch this repository. Without explicit rules, AI-generated content can drift terminology, weaken doctrine, flatten nuance, or introduce confident-sounding errors. This document prevents that.

---

## Tool Roles

Two AI tools are used in this workflow. They have distinct roles and should not be used interchangeably.

### ChatGPT — Thinking Partner and Content Architect

**What ChatGPT does:**
- Helps architect the knowledge system (document structure, terminology design, hierarchy decisions)
- Serves as a brainstorming partner for concepts, models, and frameworks
- Generates first drafts of new content based on Coach West's input and conversation
- Identifies gaps in existing content
- Helps structure complex ideas before they are written into documents

**What ChatGPT does NOT do:**
- Write directly to the repository
- Approve its own content
- Make governance or doctrine decisions without human review
- Define new terminology — it can propose; Coach West decides

**How to use ChatGPT effectively:**
- Provide it with the relevant section of doctrine or terminology before asking it to draft content
- Ask it to flag any terminology it is uncertain about
- Treat all ChatGPT output as a draft that requires review before committing
- When ChatGPT introduces a new term, evaluate whether it belongs in `terminology.md`

---

### GitHub Copilot — Repository Execution Agent

**What Copilot does:**
- Creates new files from templates and instructions
- Expands stub files with structured content
- Updates frontmatter, cross-links, and formatting
- Executes specific, well-defined document tasks in the repository
- Follows instructions to modify existing documents

**What Copilot does NOT do:**
- Override doctrine established by Coach West
- Rename or redefine terms in `terminology.md` without explicit instruction
- Approve its own changes — all changes are committed to branches or flagged for review
- Make editorial decisions — it implements decisions Coach West has made

**How to use Copilot effectively:**
- Provide Copilot with the relevant existing documents before asking it to write new content
- Be explicit about which document type (doctrine/framework/guide/etc.) is being created
- Always review Copilot-generated content before treating it as authoritative
- If Copilot introduces a term not in `terminology.md`, flag it and evaluate whether to add it

---

## What Changes Require Human Review

Not all AI-generated content carries the same risk. Use this table to determine when human review is required before a change is committed or treated as authoritative.

| Change Type | AI Tool | Review Required |
|-------------|---------|-----------------|
| New term added to `terminology.md` | Either | **Yes — Coach West approves** |
| Change to existing term definition | Either | **Yes — Coach West approves** |
| New doctrine document or major section | Either | **Yes — Coach West approves** |
| Structural change to document hierarchy | Either | **Yes — Coach West approves** |
| New framework document (substantive content) | Either | **Yes — Program coach reviews** |
| Stub/placeholder file created | Copilot | Light review — verify frontmatter and links |
| Content added to existing stub | Copilot | Review for terminology and accuracy |
| Formatting, frontmatter, link updates | Copilot | Spot check |
| Template updates | Copilot | Review that standard is preserved |
| Typos, broken links | Copilot | No formal review needed |

---

## Terminology Preservation Rules

Terminology drift is the most common way AI tools damage a knowledge system.

**Rules:**

1. **Never redefine a term locally.** If a term is in `terminology.md`, use it as defined. Do not modify or narrow the definition inside a different document.

2. **If a term is missing from `terminology.md`, add it there first.** Do not define it inline in a framework or guide.

3. **When AI introduces a new term, evaluate it.** Ask: Is this already covered by an existing term? Is this the right word? What are the implications if this term is used inconsistently elsewhere?

4. **Watch for synonym drift.** AI tools frequently introduce near-synonyms for established terms. Example: "shot release" and "shot break" mean the same thing — only one should be used. The canonical term wins.

5. **Watch for metaphor creep.** Wilco doctrine explicitly avoids ambiguous firearm metaphors in non-technical contexts. If AI introduces figurative uses of "trigger," "reload," or similar terms in non-technical writing, remove them.

6. **Preserve the impact assessment vocabulary.** The terms visual assessment, audible assessment, predictive assessment, index/feel, and hybrid assessment are specific and intentional. AI tools may simplify or collapse these into "shot calling" — do not allow that substitution.

---

## Doctrine Governance Rules for AI

AI tools do not understand doctrine. They generate plausible content. That is not the same thing.

**Rules:**

1. **Doctrine answers WHY. Frameworks answer HOW.** If AI-generated content in a framework begins to explain philosophy, move that content to doctrine. If doctrine begins to describe specific procedures, move it to a framework or operations document.

2. **AI cannot elevate content.** A draft document does not become approved because AI generated it confidently. Status lifecycle (draft → in-review → approved) applies to all content regardless of source.

3. **Cross-links must be verified.** AI tools frequently generate plausible-looking internal links that point to files that do not exist or sections that have moved. All links should be verified before committing.

4. **Frontmatter must be reviewed.** Verify `document_type`, `status`, `related_documents`, and `tags` on every AI-generated file.

5. **AI-generated content should not reference external organizations, specific athletes, or real-world entities without explicit instruction and review.** This prevents inaccurate attributions or privacy issues.

---

## Escalation: When to Stop and Ask

If an AI tool produces any of the following, stop and review with Coach West before proceeding:

- A new term that seems to replace or overlap with a term already in `terminology.md`
- Doctrine content (WHY statements) appearing in a framework or guide
- A structural change to the document hierarchy
- Content that contradicts an existing approved document
- Cross-links to files that do not exist
- Any content touching the safety doctrine

---

## Sections to Develop

- [ ] Specific prompt templates for common Copilot tasks (create stub, expand framework, update crosswalk)
- [ ] Specific prompt templates for common ChatGPT tasks (brainstorm framework, review terminology, identify gaps)
- [ ] Version of this guide for onboarding new coaches who will use AI tools
- [ ] Decision checklist for "should AI write this or should I?"

---

*Wilco Shooting Sports · AI Workflow Guide v0.1 · Draft*
