# AIDeliveryOS System Map

**Version:** 0.1  
**Status:** Public MVP  
**Review Date:** TBD  

---

## Purpose

This document describes how the public AIDeliveryOS repository is organized.

AIDeliveryOS is a Context Engineering framework focused on Implementation Readiness before development begins. The primary output is a **Project Context Package** — a structured set of documents that guides both humans and AI coding agents through discovery, decision-making, and implementation.

This system map reflects the **current public repository only**. It is the authoritative guide for where content belongs, what is in active use, and what is historical.

If you are entering this repository for the first time, read this document after `README.md` and before creating or moving files.

---

## Public Repository Structure

```text
AIDeliveryOS/
│
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── CHANGELOG.md
├── SECURITY.md
├── ROADMAP.md
├── FAQ.md
│
├── docs/
├── starter-kits/
├── examples/
├── templates/
└── archive/
```

These five directories form the active public content model for the MVP release.

---

## Directory Responsibilities

### `docs/`

Core methodology, architecture, roadmap, and system guidance.

Primary documents:

| File | Purpose |
|---|---|
| `vision.md` | Long-term direction and problem framing |
| `methodology.md` | How the Context Engineering process works |
| `architecture.md` | System model, boundaries, and design guidance |
| `technology-guidance.md` | Technology selection and engineering guidance |
| `roadmap.md` | Supplementary roadmap notes (see root `ROADMAP.md` for the official roadmap) |
| `system-overview.md` | High-level system flow and component overview |
| `system-map.md` | This document — repository organization and scope |

**Rule:** Strategic and methodological content belongs here. Do not duplicate authoritative guidance across other folders.

---

### `starter-kits/`

Project intake and startup resources.

| File | Purpose |
|---|---|
| `project-starter-template.md` | Primary project intake form for new projects |

**Rule:** Starter kits help users begin discovery and move toward a Project Context Package. They should remain practical and repeatable.

---

### `templates/`

Reusable Context Engineering templates.

| File | Purpose |
|---|---|
| `project-context-package-template.md` | Template for assembling a Project Context Package |

**Rule:** Templates define structure, not project-specific decisions. Keep them generic and reusable.

---

### `examples/`

Example Project Context Packages and reference implementations.

| Path | Purpose |
|---|---|
| `examples/README.md` | How to use and learn from the examples |
| `examples/ai-product-project/` | AI product reference package |
| `examples/marketplace-project/` | Marketplace reference package |
| `examples/saas-project/` | SaaS reference package |

**Rule:** Examples demonstrate the methodology in practice. They should reflect realistic Context Engineering workflows and Implementation Readiness outcomes.

---

### `archive/`

Historical content and previous iterations.

**Rule:** Do not treat `archive/` as active guidance. Content here is preserved for reference only and may reflect outdated structures, terminology, or approaches.

---

## Root-Level Governance Files

| File | Purpose |
|---|---|
| `README.md` | Project overview, positioning, and entry point |
| `LICENSE` | Apache License 2.0 terms |
| `CONTRIBUTING.md` | Contribution guidelines and expectations |
| `CODE_OF_CONDUCT.md` | Community standards |
| `CHANGELOG.md` | Release history and notable changes |
| `SECURITY.md` | Security policy and reporting guidance |
| `ROADMAP.md` | Validation-gated roadmap and phase progression |
| `FAQ.md` | Frequently asked questions |

**Rule:** Governance files at the repository root define how the project operates publicly. Substantive methodology belongs in `docs/`, not duplicated across governance files.

---

## Context Engineering Lifecycle

AIDeliveryOS supports a repeatable lifecycle from idea to Implementation Readiness:

```text
Idea
  ↓
Discovery
  ↓
Analysis
  ↓
Recommendations
  ↓
Project Context Package
  ↓
Implementation Readiness
  ↓
AI-Assisted Implementation
```

Repository mapping by lifecycle stage:

| Stage | Primary Location |
|---|---|
| Orientation | `README.md`, `docs/vision.md` |
| Process guidance | `docs/methodology.md`, `docs/system-overview.md` |
| Project intake | `starter-kits/project-starter-template.md` |
| Package structure | `templates/project-context-package-template.md` |
| Reference patterns | `examples/` |
| Architecture and technology decisions | `docs/architecture.md`, `docs/technology-guidance.md` |
| Readiness validation | `docs/methodology.md`, example packages |
| AI-assisted delivery | Generated Project Context Package loaded into Claude Code, Cursor, Codex, or Windsurf |

The lifecycle is evidence-driven. Each stage should produce validated context before advancing to the next.

---

## Active Public Scope

The public MVP includes:

- Context Engineering methodology and guidance in `docs/`
- Project intake via `starter-kits/`
- Reusable templates in `templates/`
- Reference Project Context Packages in `examples/`
- Open-source governance at the repository root

The current focus is **Methodology Validation** — confirming that Project Context Packages improve Implementation Readiness before investing in automation, orchestration, agents, knowledge graphs, or platform development.

What the public repository is **not** yet:

- A software platform
- An agent orchestration system
- A recommendation engine
- An automated Project Context Package generator
- An enterprise governance product

Complexity follows validation.

---

## Archived Content

The `archive/` directory contains historical material from earlier iterations of the project.

Characteristics of archived content:

- May reference deprecated folder structures or terminology
- May include experimental frameworks, engines, or prompts
- Is not maintained to the same standard as active public content
- Should not be copied into new Project Context Packages without review

When in doubt, prefer active content in `docs/`, `templates/`, `starter-kits/`, and `examples/`.

---

## Drift Prevention Rules

To keep the public repository coherent:

1. **One source of truth per concept.** Methodology lives in `docs/methodology.md`. Repository organization lives in this document.
2. **Context before code.** Do not add implementation artifacts to active public folders until the methodology phase validates the need.
3. **Templates stay generic.** Project-specific decisions belong in generated Project Context Packages, not in shared templates.
4. **Examples demonstrate readiness.** Each example should show a complete, realistic path from intake to Implementation Readiness.
5. **Archive, do not delete silently.** Deprecated content moves to `archive/` with context, not scattered across active folders.
6. **Terminology consistency.** Use **Context Engineering**, **Project Context Package**, and **Implementation Readiness** consistently across all active documents.
7. **No phantom folders.** Do not document or recreate root-level folders that are not part of the current public structure.
8. **Validation before complexity.** New directories, automation, or platform concepts require demonstrated value from real-world usage first.

---

## Current Public Structure Summary

```text
Active Public Directories
├── docs/              Core methodology, architecture, roadmap, and system guidance
├── starter-kits/      Project intake and project startup resources
├── examples/          Example Project Context Packages and reference implementations
├── templates/         Reusable Context Engineering templates
└── archive/           Historical content and previous iterations (reference only)

Root Governance
├── README.md          Entry point and project positioning
├── LICENSE            Apache License 2.0
├── CONTRIBUTING.md    Contribution guidelines
├── CODE_OF_CONDUCT.md Community standards
├── CHANGELOG.md       Release history
├── SECURITY.md        Security policy
├── ROADMAP.md         Validation-gated roadmap
└── FAQ.md             Frequently asked questions
```

**Recommended reading order for new contributors:**

1. `README.md`
2. `docs/vision.md`
3. `docs/methodology.md`
4. `docs/system-overview.md`
5. This document (`docs/system-map.md`)
6. `starter-kits/project-starter-template.md`
7. `templates/project-context-package-template.md`
8. `examples/README.md`

Better context leads to better decisions.

Better decisions lead to better software.
