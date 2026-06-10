# Vibe Coding Workflow

A reusable, dialogue-based workflow for building products from idea to production. Designed for VSCode. Stored in GitHub. Used at the start of every new project.

---

## How It Works

This workflow guides you through 10 structured steps — from discovery to QA. Each step has:
- A clear objective
- Questions the AI will ask (one at a time)
- A defined output
- A gate that must pass before moving to the next step

The AI acts as a **professional senior developer** — not a yes-man. It challenges weak assumptions, refuses to skip steps, and evaluates your answers critically.

---

## Setup for a New Project

1. Copy the `.workflow/` folder into your project root
2. Open `config.md` and fill in the project settings
3. Set `git: public` or `git: private`
   - If `private`, add `.workflow/` to your `.gitignore`
4. Start with Step 01

---

## Starting the Workflow

Paste this prompt into your AI tool (Copilot Chat, Claude, Cline, etc.):

```
You are a professional senior developer running a structured vibe coding workflow.

Load the following files:
- .workflow/config.md
- .workflow/_progress.md
- .workflow/01-discovery.md

Follow the instructions in 01-discovery.md exactly.
Ask one question at a time.
Do not skip steps or gates.
Update _progress.md automatically when each gate passes.
```

---

## Resuming a Session

If you're continuing from a previous session, paste this:

```
Load .workflow/_progress.md and continue the workflow from where we left off.
Then load the current step file and follow its instructions.
```

---

## Workflow Steps

| Step | File | Purpose |
|---|---|---|
| 01 | `01-discovery.md` | Uncover idea, problem, target user |
| 02 | `02-clarify.md` | Define scope and constraints |
| 03 | `03-spec.md` | Write the PRD |
| 04 | `04-content.md` | Confirm content assets and readiness |
| 05 | `05-risk.md` | Identify and mitigate risks |
| 06 | `06-architecture.md` | Design system architecture |
| 07 | `07-design-system.md` | Define UI design system |
| 08 | `08-stack.md` | Select technology stack |
| 09 | `09-build-plan.md` | Plan the build phase by phase |
| 10 | `10-build.md` | Execute the build |
| 11 | `11-qa.md` | Audit and fix all issues |

---

## Key Files

| File | Purpose |
|---|---|
| `config.md` | Project settings and AI behavior rules |
| `_progress.md` | Auto-updated status and context (resume from here) |
| `_decisions.md` | Log of all key decisions made by AI and user |

---

## Principles

- **One question at a time** — keeps token usage minimal and focused
- **Gate system** — AI refuses to proceed if current step is incomplete
- **No skipping** — every step exists for a reason
- **Auto-progress tracking** — `_progress.md` always reflects current state
- **Decision logging** — `_decisions.md` records why decisions were made
- **Adaptable** — works for any product type, any starting point
