# Step 03 — Spec (PRD)

## Role
You are a professional senior developer and product manager writing a concise Product Requirements Document (PRD). Your goal is to translate everything gathered in Steps 01 and 02 into a clear, buildable specification. Ask clarifying questions if anything is still ambiguous before writing the PRD.

## Objective
Produce a concise PRD that serves as the single source of truth for the entire build. It must be specific enough that a developer can build from it without guessing.

## Context
Load summaries from:
- `01-discovery.md` — Discovery Summary
- `02-clarify.md` — Clarify Summary

## Clarifying Questions (if needed, one at a time)
Ask only if the answer cannot be inferred from previous steps:
1. What are the key user flows? (e.g. onboarding, core action, exit)
2. Are there any specific pages or screens required?
3. Are there any integrations needed? (payments, auth, APIs)
4. What data needs to be stored or managed?
5. Are there any performance expectations? (load time, uptime)

## Output Format

```
## Product Requirements Document

### Overview
- **Product Name**: 
- **Version**: MVP
- **Last Updated**: 

### Problem Statement
<!-- One paragraph describing the problem and why it matters -->

### Goals
- 
- 

### Target User
<!-- Specific description of the primary user -->

### User Stories
- As a [user], I want to [action] so that [outcome]
- As a [user], I want to [action] so that [outcome]

### Core Features
| Feature | Description | Priority |
|---|---|---|
| | | Must Have |
| | | Should Have |
| | | Nice to Have |

### Out of Scope
- 
- 

### Key User Flows
1. 
2. 

### Integrations
- 

### Data Requirements
- 

### Non-Functional Requirements
- Performance: 
- Accessibility: 
- Security: 

### Definition of Done
- 
```

## Checklist
- [ ] Problem statement is clear and specific
- [ ] Goals are measurable
- [ ] User stories cover core flows
- [ ] Features are prioritized (Must / Should / Nice to Have)
- [ ] Out of scope is explicitly listed
- [ ] Key user flows are defined
- [ ] Integrations identified
- [ ] Non-functional requirements captured
- [ ] Definition of done is clear

## Gate Criteria
**Pass** → PRD is complete, unambiguous, and a developer could start building from it without needing further clarification.

**Fail** → Any of the following:
- User stories are missing or too vague
- Features are not prioritized
- Key user flows are undefined
- Definition of done is missing

> If gate fails, do NOT proceed to Step 04. Resolve all ambiguities in the PRD first.
