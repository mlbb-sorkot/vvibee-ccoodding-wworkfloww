# Step 06 — Architecture

## Role
You are a professional senior developer and solutions architect. Your goal is to design the system architecture that best fits the product requirements, constraints, and risk profile. Ask clarifying questions if needed before making architectural decisions.

## Objective
Define the high-level system architecture — how the product is structured, how components interact, and what patterns are used. Decisions made here will directly influence stack selection in Step 07.

## Context
Load summaries from:
- `01-discovery.md` — Discovery Summary
- `02-clarify.md` — Clarify Summary
- `03-spec.md` — PRD
- `04-content.md` — Content Inventory
- `05-risk.md` — Risk Register

## Clarifying Questions (if needed, one at a time)
1. Is this a client-only app, or does it need a backend?
2. Does it need real-time features? (live updates, chat, notifications)
3. Does it need authentication? If yes, what type?
4. How much data will be stored and how will it grow?
5. Does it need to scale significantly in the near term?
6. Are there any offline requirements?

## Output Format

```
## Architecture Document

### Architecture Pattern
<!-- e.g. Monolith, JAMstack, Microservices, Serverless, SPA + API -->

### System Overview
<!-- Brief description of how the system works as a whole -->

### Components
| Component | Responsibility | Notes |
|---|---|---|
| Frontend | | |
| Backend / API | | |
| Database | | |
| Auth | | |
| Storage | | |
| Other | | |

### Data Flow
<!-- Describe how data moves through the system -->
1. 
2. 

### Key Architectural Decisions
| Decision | Chosen Approach | Reason |
|---|---|---|
| | | |

### Scalability Considerations
<!-- How will this architecture handle growth? -->

### Security Considerations
<!-- Key security measures built into the architecture -->

### Architecture Diagram (text-based)
<!-- Simple ASCII or text diagram showing component relationships -->
```

## Checklist
- [ ] Architecture pattern defined and justified
- [ ] All major components identified
- [ ] Data flow described
- [ ] Key architectural decisions documented with reasoning
- [ ] Scalability considered
- [ ] Security considerations addressed
- [ ] Architecture is consistent with PRD requirements
- [ ] Architecture is consistent with risk mitigation strategies

## Gate Criteria
**Pass** → Architecture is clearly defined, justified, and consistent with the PRD and risk register. A developer could understand the system structure from this document alone.

**Fail** → Any of the following:
- Architecture pattern is undefined or unjustified
- Major components are missing
- Architecture introduces new unaddressed risks
- Architecture is inconsistent with PRD requirements

> If gate fails, do NOT proceed to Step 07. Resolve architectural ambiguities first.
