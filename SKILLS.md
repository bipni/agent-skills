## Personal Docs (pdocs)

Every project must have a `pdocs/` folder for personal, local-only documentation — never committed to the repo.

### Setup

- If `pdocs/` does not exist in the project root, create it.
- Ensure `pdocs/` is listed in the project's `.gitignore`. If `.gitignore` doesn't exist, create one and add the entry.
- Inside `pdocs/`, ensure a `workflows/` subfolder exists (create if missing): `pdocs/workflows/`.

### Writing workflows

When I ask you to "write a workflow for X":

1. Create a new Markdown file inside `pdocs/workflows/`.
2. Name the file descriptively in kebab-case based on the workflow's purpose, e.g. `deploy-to-staging.md`, `setup-local-db.md`, `release-checklist.md`.
3. Do not overwrite an existing workflow file with the same name — if one already exists, ask whether to update it or create a new version.
4. Structure the workflow file clearly, e.g.:
   - Title (`# Workflow: <name>`)
   - Short description of what it's for
   - Numbered steps
   - Any relevant commands, gotchas, or notes

### Notes

- `pdocs/` is personal scratch space — treat its contents as notes/history for me, not project documentation meant for the team.
- Never suggest committing `pdocs/` to version control.
