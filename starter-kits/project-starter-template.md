# Project Context Intake Template

**Version:** 0.1 [DRAFT]  
**OS Reference:** `ai-coding-operating-system.md`  

---

## Instructions

Copy this file into a new project workspace as `projects/[project-name]/project.md`. Fill in every field before any architecture work begins. This document becomes the single source of truth for the project's identity, goals, and initial shape.

Do not leave `[TBD]` in fields that can be answered at project start. Use `[TBD — decision by DATE]` only for genuinely open items with a deadline.

---

## What This Document Produces

This intake document is the starting point for every AIDeliveryOS project.

After completion, it can be used to generate a Project Context Package containing:

- PROJECT_BRIEF.md
- PRD.md
- ARCHITECTURE.md
- ROADMAP.md
- RISKS.md
- CLAUDE.md
- AGENTS.md
- CODING_STANDARDS.md
- AUDIT_REQUIREMENTS.md

These documents become the operating instructions and guardrails for AI coding agents.

---

## Document Header

| Field | Value |
|-------|-------|
| Project Name | [Project Name] |
| Project Code | [Short code, e.g., GEO-CORE] |
| Owner | [Owner Name] |
| Status | [Idea / Discovery / Architecture / Build / Audit / Release / Maintenance] |
| Version | 0.1 |
| Created Date | [Date] |
| Target Launch | [Date or TBD] |
| Review Date | [Date — set at project start] |

---

## Project Classification

> Classify the project before discovery begins.

### Project Category

- [ ] SaaS
- [ ] Marketplace
- [ ] AI Application
- [ ] Agent System
- [ ] RAG System
- [ ] Knowledge Graph
- [ ] Internal Tool
- [ ] Analytics Platform
- [ ] GEO Platform
- [ ] Workflow Automation
- [ ] Other

### Complexity Estimate

- [ ] Low
- [ ] Medium
- [ ] High
- [ ] Enterprise

### Expected Delivery Horizon

- [ ] Less than 30 Days
- [ ] 30-90 Days
- [ ] 3-6 Months
- [ ] 6-12 Months
- [ ] 12+ Months

### AI Readiness

- [ ] No AI Components
- [ ] AI Assisted Features
- [ ] AI Native Product
- [ ] Agentic System

---

## 1. Business Objective

> What business outcome must this project achieve? Be specific — tie it to revenue, retention, acquisition, or cost.

*[Describe the business objective in 2–4 sentences. Avoid technical language. This should be readable by a non-technical stakeholder.]*

**Success looks like:**
- [Measurable outcome 1]
- [Measurable outcome 2]

---

## 2. Problem Statement

> What problem does this project solve? From whose perspective?

**Customer problem:**  
*[Describe the problem from the customer's point of view.]*

**Business problem:**  
*[Describe the business problem this creates if unsolved.]*

**Evidence this problem is real:**
- [Data point, user quote, or market evidence 1]
- [Data point 2]

---

## Context Gap Assessment

> What information is currently missing?

| Area | Known | Unknown |
|--------|--------|--------|
| Customer | | |
| Business Model | | |
| Requirements | | |
| Data Sources | | |
| Technology | | |
| Risks | | |
| Compliance | | |

### Largest Unknown

[Describe the single biggest unknown.]

### Validation Needed

[Describe what must be learned before architecture begins.]

---

## 3. User Personas

> Who uses this system? Define each persona specifically enough to make product decisions.

### Persona 1: [Name]

| Attribute | Value |
|-----------|-------|
| Role | [Job title] |
| Company type | [e.g., Mid-market B2B SaaS] |
| Goal | [What they are trying to accomplish] |
| Pain point | [What problem they face today] |
| Technical proficiency | [High / Medium / Low] |
| Primary use case | [How they will use this product] |

### Persona 2: [Name]

| Attribute | Value |
|-----------|-------|
| Role | |
| Company type | |
| Goal | |
| Pain point | |
| Technical proficiency | |
| Primary use case | |

---

## 4. Product Type

Select the product type(s) that apply:

- [ ] AI SaaS application
- [ ] GEO / AI search visibility platform
- [ ] RAG system
- [ ] Knowledge graph system
- [ ] Agent system
- [ ] Reporting and analytics platform
- [ ] Marketplace
- [ ] API platform
- [ ] Search platform
- [ ] Workflow automation
- [ ] Other: [Describe]

---

## 5. Product Characteristics

> Select all characteristics that apply. AIDeliveryOS uses these inputs to recommend architecture patterns and implementation approaches.

- [ ] Multi-tenant SaaS
- [ ] Marketplace
- [ ] Search experience
- [ ] Internal tool
- [ ] AI-powered features
- [ ] Mobile application
- [ ] Workflow automation
- [ ] Reporting and analytics
- [ ] Public API
- [ ] Knowledge system
- [ ] Agent system
- [ ] Enterprise software
- [ ] Consumer application
- [ ] Other: [Describe]

**Additional notes:**
*[Describe any characteristics that may affect architecture recommendations.]*

---

## AI Coding Environment

> Which environment will use the generated Project Context Package?

### Primary AI Coding Tool

- [ ] Claude Code
- [ ] Cursor
- [ ] Codex
- [ ] Windsurf
- [ ] Other: [Specify]

### Development Model

- [ ] Single AI agent
- [ ] Multi-agent workflow
- [ ] Human + AI pair programming

### Repository Type

- [ ] New project
- [ ] Existing repository

---

## 6. AI Capabilities Required

> Which AI capabilities does this project require?

| Capability | Required | Pattern Reference |
|-----------|---------|-----------------|
| RAG / retrieval-augmented generation | Yes / No | `ai/rag-patterns.md` |
| Vector search | Yes / No | `ai/vector-strategy.md` |
| Knowledge graph | Yes / No | `ai/knowledge-graph-patterns.md` |
| Multi-agent orchestration | Yes / No | `ai/agent-patterns.md` |
| Citation intelligence | Yes / No | `ai/citation-strategy.md` |
| Prompt pipelines | Yes / No | `ai/prompt-patterns.md` |
| LLM generation | Yes / No | `ai/model-selection-framework.md` |
| Entity extraction | Yes / No | `data-models/entity-model.md` |
| Evaluation pipeline | Yes / No | `evaluation/evaluation-framework.md` |

---

## 7. Data Sources

> What data does this system ingest, process, or generate?

| Source | Type | Frequency | Volume | Owner |
|--------|------|-----------|--------|-------|
| [Source 1] | [web / api / db / upload] | [real-time / hourly / daily] | [estimate] | [Team] |
| [Source 2] | | | | |

**Data residency requirements:**  
*[Any geographic or compliance constraints on where data is stored or processed?]*

**PII considerations:**  
*[Does any data contain personally identifiable information? If yes, document handling requirements.]*

---

## 8. Success Metrics

> How will you know this project succeeded? Define metrics before building.

| Metric | Baseline | Target | Timeframe | Owner |
|--------|---------|--------|-----------|-------|
| [North star metric] | [Value] | [Value] | [By when] | [Name] |
| [AI quality metric] | [Value] | [Value] | [By when] | [Name] |
| [Business metric] | [Value] | [Value] | [By when] | [Name] |
| [Operational metric] | [Value] | [Value] | [By when] | [Name] |

**AI-specific quality metrics:**

| Metric | Target |
|--------|--------|
| Retrieval Recall@5 | [e.g., >80%] |
| Citation accuracy | [e.g., >90%] |
| P95 response latency | [e.g., <3s] |
| Hallucination rate | [e.g., <5%] |

---

## Success Metric Hierarchy

### Business Outcomes

- Revenue
- Retention
- Acquisition
- Cost Savings

### Customer Outcomes

- Adoption
- Engagement
- Satisfaction
- Task Success

### Leading Indicators

- Activation
- Usage
- Conversion
- Workflow Completion

### Operational Metrics

- Reliability
- Performance
- Cost
- Quality

---

## 9. Constraints

> What constraints shape the design before architecture begins?

| Category | Constraint |
|----------|-----------|
| Budget | [Monthly infrastructure budget estimate] |
| Timeline | [Hard deadline if any] |
| Team size | [Number of engineers] |
| Compliance | [GDPR / HIPAA / SOC2 / None] |
| Geography | [Data residency requirements] |
| Existing infrastructure | [Existing tools that must be reused] |
| Performance | [Latency or throughput requirements] |

---

## Assumptions Register

> Document assumptions before they become hidden risks.

| Assumption | Confidence | Validation Method |
|-----------|-----------|------------------|
| | High / Medium / Low | |
| | High / Medium / Low | |

### Critical Assumptions

List assumptions that would invalidate the project if proven false.

---

## 10. Risks

> What could prevent this project from succeeding?

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk 1] | High / Med / Low | High / Med / Low | [Mitigation] |
| [Risk 2] | | | |
| [Risk 3] | | | |

---

## 11. Dependencies

> What must exist or be decided before this project can proceed?

| Dependency | Owner | Required By | Status |
|-----------|-------|------------|--------|
| [Dependency 1] | [Name] | [Date] | [Status] |
| [Dependency 2] | | | |

---

## 12. Phase 1 Definition

> What is the first phase of work? Fill this in before any code is written.

**Phase 1 Goal:**  
*[One sentence describing what Phase 1 must achieve.]*

**Phase 1 Scope:**
- [In-scope item 1]
- [In-scope item 2]

**Phase 1 Out of Scope:**
- [Out-of-scope item 1]
- [Out-of-scope item 2]

**Phase 1 Exit Gate:**  
*[Specific, testable condition that must be true before Phase 1 is complete.]*

**Phase 1 Target Date:** [Date]

**Phase 1 Owner:** [Name]

For full phase definition, use the template in `governance/phase-execution-protocol.md`.

---

## Implementation Readiness

### Architecture Ready?

- [ ] Yes
- [ ] No

### Discovery Complete?

- [ ] Yes
- [ ] No

### Major Unknowns Resolved?

- [ ] Yes
- [ ] No

### Stakeholder Alignment Confirmed?

- [ ] Yes
- [ ] No

### Recommended Next Action

- [ ] Continue Discovery
- [ ] Begin Architecture
- [ ] Perform Validation
- [ ] Build MVP
- [ ] Re-scope Project

---

## Context Readiness Assessment

> Validate that enough information exists before architecture and implementation begin.

| Question | Yes | No |
|-----------|-----|----|
| Business problem clearly defined? | [ ] | [ ] |
| Target users identified? | [ ] | [ ] |
| Success metrics defined? | [ ] | [ ] |
| MVP scope defined? | [ ] | [ ] |
| Constraints documented? | [ ] | [ ] |
| Dependencies identified? | [ ] | [ ] |
| Major risks documented? | [ ] | [ ] |

**Context Readiness Score:** ____ / 100

Projects should ideally score 80 or higher before architecture work begins.

---

## 13. Open Questions

> What is unresolved and must be answered before architecture begins?

| Question | Owner | Due Date |
|---------|-------|---------|
| [Question 1] | [Name] | [Date] |
| [Question 2] | [Name] | [Date] |

---

## 14. Related Documents

| Document | Link |
|----------|------|
| PRD | [Link] |
| Architecture doc | [Link] |
| Roadmap | [Link] |
| Design files | [Link] |
