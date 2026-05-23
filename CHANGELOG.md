# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.1] - 2026-05-23

### Added
- 🆕 Added the custom `AGS-Git-docer` agent skill at `.agents/skills/ags-git-docer/SKILL.md` to automate README and CHANGELOG updates and sync them to remote.

## [1.0.0] - 2026-05-23

### Added
- 🆕 Initialized the workspace as a Git repository and connected it to `https://github.com/ASoudy/AGS.git`.
- 🆕 Committed initial reference skills under `my_skills_reference/` (covering Web Dev, Planning, Marketing, and CI/CD).
- 🆕 Installed active workspace agent skills: `find-skills` and `create-readme` in `.agents/skills/`.
- 🆕 Created a comprehensive root `README.md` describing the workspace structure, reference indexes, and getting started guides.

### Changed
- 🔄 Converted all embedded libraries in `claude_skills_libraries/` (including Marketing Skills, Wondelai Product & Strategy, Anthropic PPTX, etc.) from git submodules/gitlinks to fully tracked local hardcopies for offline backup safety.
- 🔄 Changed the `AGAS/` folder (local copy of the Awesome Skills repository) from a Git-ignored folder to a fully tracked local hardcopy in the main repository.
- 📝 Updated the root `README.md` to reflect that both `AGAS/` and `claude_skills_libraries/` are now directly tracked in the repository.
