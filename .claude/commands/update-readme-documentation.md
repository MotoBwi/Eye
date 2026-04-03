---
name: update-readme-documentation
description: Workflow command scaffold for update-readme-documentation in Eye.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /update-readme-documentation

Use this workflow when working on **update-readme-documentation** in `Eye`.

## Goal

Updates project documentation by modifying the README.md file, such as adding, updating, or removing content.

## Common Files

- `README.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Open README.md
- Edit content (add, update, or remove sections, badges, links, etc.)
- Commit the changes with a descriptive message

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.