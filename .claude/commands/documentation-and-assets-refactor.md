---
name: documentation-and-assets-refactor
description: Workflow command scaffold for documentation-and-assets-refactor in Eye.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /documentation-and-assets-refactor

Use this workflow when working on **documentation-and-assets-refactor** in `Eye`.

## Goal

Refactor or update documentation and static image assets.

## Common Files

- `README.md`
- `README-EN.md`
- `static/image/*`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Update README files and documentation.
- Add or replace static image assets in the static/image directory.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.