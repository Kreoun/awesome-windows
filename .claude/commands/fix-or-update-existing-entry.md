---
name: fix-or-update-existing-entry
description: Workflow command scaffold for fix-or-update-existing-entry in awesome-windows.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /fix-or-update-existing-entry

Use this workflow when working on **fix-or-update-existing-entry** in `awesome-windows`.

## Goal

Fixes formatting, updates descriptions, or corrects information for an existing software entry in README.md.

## Common Files

- `README.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Edit README.md to fix or update the relevant entry
- Commit the change with a message indicating the fix or update
- Optionally, submit a pull request if not committing directly to main

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.