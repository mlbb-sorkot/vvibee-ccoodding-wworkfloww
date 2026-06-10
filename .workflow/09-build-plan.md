# Step 09 — Build Plan

## Role
You are a professional senior developer creating a detailed, executable build plan. Break down the entire build into logical phases and tasks. Think about dependencies, order of execution, and what must be built before what.

## Objective
Produce a structured build plan that guides the coding phase (Step 09) with clear tasks, phases, and priorities. This plan prevents random or unstructured coding.

## Context
Load summaries from:
- `03-spec.md` — PRD (features, user stories)
- `04-content.md` — Content Inventory (content readiness, blocking items)
- `06-architecture.md` — Architecture (components)
- `07-design-system.md` — Design System (UI components needed)
- `08-stack.md` — Stack (technology choices)

## Build Phases

Structure the build in the following order:
1. **Foundation** — Project setup, configuration, base structure
2. **Core Infrastructure** — Auth, database, routing, layout
3. **Feature Development** — Build features by priority (Must Have first)
4. **UI Polish** — Apply design system, responsive design
5. **Integration** — Connect all parts, test flows end-to-end
6. **Pre-QA Cleanup** — Code cleanup, error handling, edge cases

## Output Format

```
## Build Plan

### Phase 1 — Foundation
- [ ] Initialize project with chosen stack
- [ ] Configure environment variables
- [ ] Set up version control and branching strategy
- [ ] Configure linting and formatting
- [ ] Set up folder structure
- [ ] Configure CI/CD pipeline (if applicable)

### Phase 2 — Core Infrastructure
- [ ] Set up routing structure
- [ ] Implement base layout and navigation
- [ ] Set up database and migrations (if applicable)
- [ ] Implement authentication (if applicable)
- [ ] Set up API structure (if applicable)
- [ ] Implement design system tokens (colors, typography, spacing)

### Phase 3 — Feature Development

#### Must Have
- [ ] <!-- Feature 1 -->
  - [ ] <!-- Sub-task -->
  - [ ] <!-- Sub-task -->
- [ ] <!-- Feature 2 -->
  - [ ] <!-- Sub-task -->

#### Should Have
- [ ] <!-- Feature -->

#### Nice to Have
- [ ] <!-- Feature -->

### Phase 4 — UI Polish
- [ ] Apply full design system across all components
- [ ] Implement responsive design (mobile, tablet, desktop)
- [ ] Add loading states
- [ ] Add empty states
- [ ] Add error states
- [ ] Micro-interactions and transitions

### Phase 5 — Integration
- [ ] Connect all features end-to-end
- [ ] Test all user flows from PRD
- [ ] Verify all integrations (APIs, auth, database)

### Phase 6 — Pre-QA Cleanup
- [ ] Remove console logs and debug code
- [ ] Handle all edge cases
- [ ] Add proper error handling
- [ ] Performance check
- [ ] Code review and cleanup

---

### Build Order Summary
<!-- Numbered list of the logical order to build things -->
1. 
2. 
3. 

### Estimated Complexity
| Phase | Complexity | Notes |
|---|---|---|
| Foundation | Low / Medium / High | |
| Core Infrastructure | Low / Medium / High | |
| Feature Development | Low / Medium / High | |
| UI Polish | Low / Medium / High | |
| Integration | Low / Medium / High | |
| Pre-QA Cleanup | Low / Medium / High | |
```

## Checklist
- [ ] All 6 phases defined
- [ ] All PRD features are represented as tasks
- [ ] Tasks are ordered by dependency (no task requires an uncompleted prerequisite)
- [ ] Must Have features are in Phase 3 before Should Have and Nice to Have
- [ ] UI polish is a separate phase (not mixed with feature development)
- [ ] Pre-QA cleanup phase is included
- [ ] Build order summary is logical

## Gate Criteria
**Pass** → Build plan is complete, all PRD features are covered, tasks are ordered logically, and a developer can start Phase 1 immediately without further questions.

**Fail** → Any of the following:
- PRD features are missing from the plan
- Tasks have unresolved dependencies
- No clear starting point
- UI work is mixed into feature development without structure

> If gate fails, do NOT proceed to Step 10. Resolve the build plan before starting to code.
