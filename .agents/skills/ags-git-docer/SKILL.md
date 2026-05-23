---
name: ags-git-docer
description: "Automatically inspects the local Git repository history, classifies new changes following the Keep a Changelog standard, and updates README.md and CHANGELOG.md before committing and pushing the updates."
risk: safe
source: personal
date_added: "2026-05-23"
---

# AGS-Git-docer

## Overview
This skill automates documenting and syncing recent changes in the repository. It examines Git commits, classifies them into Keep a Changelog categories, updates `CHANGELOG.md` and `README.md`, and pushes the updates to the remote repository.

## Dependencies
- `wiki-changelog` - For changelog formatting and classification standards
- `create-readme` - For checking and styling the root README layout

## Quick Start
To trigger this skill, ask the agent:
> "Run AGS-Git-docer to update documentation"

## Workflow

### 1. Check for Git History
- Run `git log -n 10 --oneline` to retrieve the recent commits since the last update of `CHANGELOG.md`.
- Compare this with the last version/date documented in `CHANGELOG.md`.
- If there are no new commits or changes, state: *"No new updates detected. Documentation is up to date."* and stop.

### 2. Classify the Changes
Group the new commits according to the following categories:
- 🆕 **Added**: For new features, folders, or files (e.g. new skills).
- 🔄 **Changed**: For updates to existing setups, folders, or files (e.g. converting submodules to hardcopies).
- 🐛 **Fixed**: For bug fixes.
- 📝 **Docs**: For documentation improvements.
- 🔧 **Config**: For environment/git setup adjustments (e.g. updating `.gitignore`).

### 3. Update CHANGELOG.md
- Open `CHANGELOG.md` in the root workspace.
- Append a new version section (incrementing the patch or minor version, e.g. `[1.0.1] - YYYY-MM-DD`).
- Add the categorized list of changes under their respective sub-headings (e.g. `### Added`, `### Changed`).

### 4. Verify and Update README.md
- Review the root `README.md`.
- Check if the project structure, dependencies, or getting started instructions changed in the new updates.
- If changes are needed, apply the `create-readme` rules to update the descriptions and ensure the formatting (GFM and admonitions) remains modern and appealing.

### 5. Git Commit and Push
- Stage the changes: `git add CHANGELOG.md README.md` (and `.gitignore` if changed).
- Commit with a descriptive message like `Update docs for release [version]`.
- Push the changes to origin: `git push`.

### 6. Error Handling
- If the `git push` command fails (e.g., authentication, permissions, or merge conflicts): **Stop immediately and ask the user for guidance.** Do not attempt automatic pulls or force-pushes.

## Common Mistakes
- **Over-summarizing**: Grouping distinct changes under a single generic bullet. Keep descriptions detailed and precise.
- **Skipping Git verification**: Not checking the logs, which can lead to undocumented commits or duplicate entries.
- **Silent push failures**: Proceeding when `git push` exits with a non-zero code. Always check the command result.
