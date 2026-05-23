# AGS (Antigravity Skills Workspace)

*Curated personal catalog and workspace for AI Agent Skills.*

This repository functions as a centralized workspace and reference directory for managing and using **AI Agent Skills** compatible with the **Skills CLI** (`npx skills`) and AI agents such as **Antigravity** and **Claude Code**. It contains a custom reference catalog, third-party skills libraries, and active workspace agent skills.

---

## Workspace Structure

The workspace is organized as follows:
*   **`.agents/skills/`**: Core agent skills installed locally in the workspace (e.g., `find-skills`, `create-readme`).
*   **`claude_skills_libraries/`**: Cloned repositories of the **Top 8 Claude Skills for Entrepreneurs, Startup Founders, and Solopreneurs** (based on Snyk's curation).
*   **`my_skills_reference/`**: Curated lists and indexes categorized for quick developer reference.
*   **`AGAS/`** *(Git Ignored)*: A local copy of the Awesome Skills repository (`antigravity-awesome-skills`) used as a primary source for the personal reference index.

---

## Skills Reference Catalog

The [`my_skills_reference/`](my_skills_reference/) directory contains curated lists categorizing different agent skills:

1.  **[Web Development & UI/UX](my_skills_reference/web_development_skills.md)**: Astro, React, WordPress, and GraphQL skills.
2.  **[Planning & Business Management](my_skills_reference/planning_business_skills.md)**: Product design, requirements elicitation, and financial frameworks.
3.  **[Marketing, Sales & Copywriting](my_skills_reference/marketing_sales_skills.md)**: Growth engineering, copywriting, and content polishing.
4.  **[GitHub & CI/CD Pipelines](my_skills_reference/github_cicd_skills.md)**: Workflow automation, actions safety, and code deployment.

> [!NOTE]
> These catalogs contain direct file links pointing to your local `AGAS/` directory for fast offline access and reference.

---

## Cloned Libraries

The [`claude_skills_libraries/`](claude_skills_libraries/) directory tracks recommended modular prompt instruction sets (`SKILL.md`) for entrepreneurship, product management, and development:

*   **Marketing Skills (Corey Haines)**: Growth execution, launching, and copywriting.
*   **Wondelai Product & Strategy**: Product design loops (Hooked model, StoryBrand, JTBD).
*   **Anthropic PPTX Skill**: Programmatic PowerPoint generation.
*   **SaaS Metrics Coach (nginity-skills-library)**: Financial calculators and CFO modeling.
*   **Claude Skills Library (nginity)**: Large multi-domain business and product toolbox.
*   **Landing Page Mastery**: Spanish conversion copy templates and landing page design rules.
*   **Anthropic Skill Creator**: Meta-skill to author your own standard agent skills.
*   **Snyk Fix**: Automated vulnerability scanning and code remediation.

> [!IMPORTANT]
> The libraries in `claude_skills_libraries/` are tracked as embedded repositories (gitlinks) to preserve their respective git configurations while remaining easily referenceable.

---

## Getting Started

### Prerequisites

To manage and install skills in this workspace, ensure you have the Skills CLI:

```bash
npx skills --help
```

### Searching and Installing Skills

You can find new skills from the open ecosystem using the locally installed `find-skills` skill:

```bash
npx skills find <query>
```

To install a skill locally into this workspace:

```bash
npx skills add <owner/repo@skill> -y
```

> [!TIP]
> Use the `-g` flag to install a skill globally (user-level) instead of locally in the `.agents/skills/` directory.
