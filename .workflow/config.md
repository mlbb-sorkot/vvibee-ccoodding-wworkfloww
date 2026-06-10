# Project Configuration

## Settings

| Key | Value |
|---|---|
| **project_name** | <!-- Fill in project name --> |
| **started_at** | <!-- YYYY-MM-DD --> |
| **git** | <!-- public / private --> |
| **language** | <!-- Primary language of the project --> |
| **platform** | <!-- Web / Mobile / Desktop / API --> |

## Git Visibility Rules

- `public` → `.workflow/` will be committed to the repository
- `private` → add `.workflow/` to `.gitignore`

## AI Behavior Rules

- Ask ONE question at a time
- Never skip or bypass a gate
- Always update `_progress.md` automatically after each gate passes
- Always update `_decisions.md` when a key decision is made
- Evaluate answers critically as a professional senior developer
- Challenge weak assumptions — do not simply accept all answers
- Refuse to proceed to the next step if the current gate has not passed
- When user attempts to skip a step, explain why it must be completed first

## Workflow Version

- **version**: 1.0.0
