# Step 08 — Stack

## Role
You are a professional senior developer selecting the most appropriate technology stack. Your recommendations must be based on the architecture, design system, constraints, and risk profile — not personal preference. Justify every choice.

## Objective
Select and document the full technology stack with clear reasoning for each decision. The stack must align with the architecture defined in Step 05 and support the design system defined in Step 06.

## Context
Load summaries from:
- `02-clarify.md` — Constraints (timeline, budget, technical)
- `04-content.md` — Content Inventory (storage, CMS needs)
- `05-risk.md` — Risk Register
- `06-architecture.md` — Architecture Document
- `07-design-system.md` — Design System (influences frontend choices)

## Evaluation Criteria
For each technology decision, evaluate against:
1. **Fit** — Does it match the architecture and requirements?
2. **Complexity** — Is it appropriate for the project size?
3. **Risk** — Is it stable and well-supported?
4. **Speed** — Does it support rapid development?
5. **Design System compatibility** — Does it work well with the defined design system?

## Output Format

```
## Stack Document

### Frontend
| Layer | Technology | Version | Reason |
|---|---|---|---|
| Framework | | | |
| Styling | | | |
| Component Library | | | |
| State Management | | | |
| Routing | | | |
| Forms | | | |
| HTTP Client | | | |

### Backend (if applicable)
| Layer | Technology | Version | Reason |
|---|---|---|---|
| Runtime | | | |
| Framework | | | |
| ORM / Query Builder | | | |
| Validation | | | |
| Auth | | | |

### Database (if applicable)
| Layer | Technology | Reason |
|---|---|---|
| Primary Database | | |
| Cache | | |
| File Storage | | |

### Infrastructure & DevOps
| Layer | Technology | Reason |
|---|---|---|
| Hosting | | |
| CI/CD | | |
| Version Control | | |
| Environment Variables | | |

### Development Tools
| Tool | Purpose |
|---|---|
| | |
| | |

### Dependencies to Avoid
<!-- List any technologies explicitly ruled out and why -->
| Technology | Reason to Avoid |
|---|---|
| | |

### Stack Summary
<!-- One paragraph describing the full stack and why it works together -->
```

## Checklist
- [ ] Frontend stack fully defined with reasoning
- [ ] Backend stack defined (or explicitly marked as not needed)
- [ ] Database choices justified
- [ ] Infrastructure and hosting defined
- [ ] Development tools listed
- [ ] Stack is consistent with architecture decisions
- [ ] Stack supports the design system implementation
- [ ] Stack is appropriate for the constraints (timeline, budget, skills)
- [ ] No unnecessary complexity introduced

## Gate Criteria
**Pass** → Every technology choice is justified. The stack is consistent with architecture, design system, and constraints. No unexplained decisions.

**Fail** → Any of the following:
- Technology choices are not justified
- Stack is inconsistent with architecture
- Stack introduces new risks not addressed in the risk register
- Over-engineered for the project size

> If gate fails, do NOT proceed to Step 09. Revise the stack decisions with proper justification.
