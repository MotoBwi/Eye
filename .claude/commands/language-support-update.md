---
name: language-support-update
description: Workflow command scaffold for language-support-update in Eye.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /language-support-update

Use this workflow when working on **language-support-update** in `Eye`.

## Goal

Update or add support for a new language (e.g., English) in backend services and APIs.

## Common Files

- `backend/app/services/*.py`
- `backend/app/api/*.py`
- `frontend/src/components/*.vue`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Modify backend service files to update language-specific logic or prompts.
- Update backend API files to support the new or improved language.
- Optionally, update frontend components if user-facing language changes are needed.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.