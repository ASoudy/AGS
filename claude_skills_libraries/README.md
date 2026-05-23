# Claude Agent Skills Library Index & Guide

This directory contains the cloned repositories for the **Top 8 Claude Skills for Entrepreneurs, Startup Founders, and Solopreneurs** (based on Snyk's article). These skills act as modular prompt instruction sets (`SKILL.md`) that teach AI agents (such as Claude Code) domain-specific workflows and strategic frameworks.

---

## 📂 Folders & Skills Mapping

Below is the directory map of the cloned libraries and where to locate the specific skills recommended in the article:

| # | Skill / Collection | Source Repo | Local Directory | Key Skill Folder(s) / Path |
|---|--------------------|-------------|-----------------|-----------------------------|
| **1** | **Marketing Skills** (Corey Haines) | `coreyhaines31/marketingskills` | [`marketing-skills-coreyhaines`](file:///d:/A/Local/AGS/claude_skills_libraries/marketing-skills-coreyhaines) | `skills/` (25 marketing skills, e.g., `copywriting-cro`, `seo-audit`, `launch-strategy`) |
| **2** | **Wondelai Product & Strategy** | `wondelai/skills` | [`wondelai-product-strategy`](file:///d:/A/Local/AGS/claude_skills_libraries/wondelai-product-strategy) | Root directory (11 strategy framework skills including Jobs-to-be-Done, StoryBrand, Hooked UX) |
| **3** | **Anthropic PPTX Skill** | `anthropics/skills` | [`anthropic-skills`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills) | [`skills/pptx/`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills/skills/pptx/) (Official PPTX generator/reader) |
| **4** | **SaaS Financial Projections** | *Private/Deleted* | *Unavailable* | *Alternative:* [`nginity-skills-library/finance/skills/saas-metrics-coach`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library/finance/skills/saas-metrics-coach/) |
| **5** | **Claude Skills Library** (nginity) | `alirezarezvani/claude-skills` | [`nginity-skills-library`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library) | `business-growth/`, `product-team/`, `marketing/`, `finance/` (48 total skills across 7 bundles) |
| **6** | **Landing Page Mastery** | `alexdcd/Mafia-Claude-Skills` | [`landing-page-mastery`](file:///d:/A/Local/AGS/claude_skills_libraries/landing-page-mastery) | [`skills/landing-page-mastery/`](file:///d:/A/Local/AGS/claude_skills_libraries/landing-page-mastery/skills/landing-page-mastery/) (High-conversion landing page framework - Spanish) |
| **7** | **Anthropic Skill Creator** | `anthropics/skills` | [`anthropic-skills`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills) | [`skills/skill-creator/`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills/skills/skill-creator/) (Official meta-skill for building custom skills) |
| **8** | **Snyk Fix** | `snyk/studio-recipes` | [`snyk-fix`](file:///d:/A/Local/AGS/claude_skills_libraries/snyk-fix) | `command_directives/synchronous_remediation/claude_code/skills/snyk-fix/` (Automated security scanning & fix) |

---

## 🔍 Detailed Understanding of Each Library

### 1. Marketing Skills by Corey Haines
*   **Focus:** Core marketing execution, launch planning, and copywriting.
*   **Key Files:**
    - [`copywriting-cro/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/marketing-skills-coreyhaines/skills/copywriting-cro/SKILL.md): Conversional copywriting templates, copy review checkpoints, and heuristics.
    - [`seo-audit/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/marketing-skills-coreyhaines/skills/seo-audit/SKILL.md): Step-by-step checklist to conduct SEO Audits, optimize keyword strategy, and technical crawling.
    - [`launch-strategy/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/marketing-skills-coreyhaines/skills/launch-strategy/SKILL.md): Launch checklist across Product Hunt, Hacker News, email marketing, and social media.

### 2. Wondelai Product & Strategy Skills
*   **Focus:** Product design strategy and business model validation using popular conceptual frameworks.
*   **Key Files:**
    - [`jobs-to-be-done/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/wondelai-product-strategy/jobs-to-be-done/SKILL.md): Customer interview script generator, timeline builder, and push-pull forces analyzer.
    - [`storybrand/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/wondelai-product-strategy/storybrand/SKILL.md): A workflow to create a clear "StoryBrand BrandScript" (Character -> Problem -> Guide -> Plan -> CTA -> Avoid Failure -> Achieve Success).
    - [`hooked-ux/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/wondelai-product-strategy/hooked-ux/SKILL.md): Analyzing product loops based on Nir Eyal's Hooked model (Trigger -> Action -> Variable Reward -> Investment).

### 3. Anthropic PPTX Skill
*   **Focus:** Creating, editing, and reading Microsoft PowerPoint (.pptx) presentations dynamically from text prompts.
*   **Key Files:**
    - [`skills/pptx/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills/skills/pptx/SKILL.md): Instructions for slide layouts, slide notes, text wrapping, and slide design.
    - [`skills/pptx/scripts/pptx_util.py`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills/skills/pptx/scripts/pptx_util.py): The Python script that interacts with `python-pptx` to build actual slides programmatically.

### 4. SaaS Financial Projections (Alternative)
*   **Note:** The original repository `founderjourney/claude-skills` is currently unavailable (private or deleted).
*   **Best Alternative:** We recommend the **SaaS Metrics Coach** skill found within Alireza Rezvani's library:
    - [`saas-metrics-coach/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library/finance/skills/saas-metrics-coach/SKILL.md): This functions as a virtual SaaS CFO, taking inputs (MRR, churn, CAC, ARPU, gross margin) and using calculators to generate unit economics, CAC paybacks, Quick Ratios, and forward projections.
    - [`saas-metrics-coach/scripts/metrics_calculator.py`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library/finance/skills/saas-metrics-coach/scripts/metrics_calculator.py): Python utility script to run interactive calculations.

### 5. Claude Skills Library by Nginity (Alireza Rezvani)
*   **Focus:** A massive multi-domain toolbox with 48 skills for engineering, business development, product management, and advisory workflows.
*   **Key Folders:**
    - [`product-team/skills/`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library/product-team/skills/): Product roadmap planners, PRD writers, user story mapping.
    - [`c-level-advisor/skills/`](file:///d:/A/Local/AGS/claude_skills_libraries/nginity-skills-library/c-level-advisor/skills/): Business strategy, OKR planners, and negotiation coaches.

### 6. Landing Page Mastery
*   **Focus:** A structured expert system specifically optimized for high-converting landing pages.
*   **Note:** Prompts are in Spanish by default, but you can explicitly ask Claude to respond in English.
*   **Key Files:**
    - [`skills/landing-page-mastery/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/landing-page-mastery/skills/landing-page-mastery/SKILL.md): The core copywriting, structure, design guidelines, and audit checklist.
    - [`references/copywriting.md`](file:///d:/A/Local/AGS/claude_skills_libraries/landing-page-mastery/skills/landing-page-mastery/references/copywriting.md): Specific templates (PAS, AIDA, Hero, CTAs) and landing page patterns.

### 7. Anthropic Skill Creator
*   **Focus:** A meta-skill designed to help users generate well-formed, compliant custom Claude Skills.
*   **Key Files:**
    - [`skills/skill-creator/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/anthropic-skills/skills/skill-creator/SKILL.md): Guides you in defining skills, including naming conventions, description rules, formatting the `SKILL.md` file, defining tools, reference documents, and permissions.

### 8. Snyk Fix
*   **Focus:** Integrating automated vulnerability scanning and code fixing in active terminal/agent workflows.
*   **Key Files:**
    - [`snyk-fix/SKILL.md`](file:///d:/A/Local/AGS/claude_skills_libraries/snyk-fix/command_directives/synchronous_remediation/claude_code/skills/snyk-fix/SKILL.md): Commands for scanning dependencies, fixing security vulnerabilities, and compiling reports.

---

## ⚙️ How to Install and Use a Claude Skill

Claude Code reads user-level skills from `~/.claude/skills/` and project-level skills from `.claude/skills/` inside your project root.

To install any of the skills:
1. Create a directory named `.claude/skills/<skill-name>` in your project root.
2. Copy the corresponding `SKILL.md` (and any accompanying folders like `references/` or `scripts/`) into that folder.
3. Restart Claude Code, or ask Claude to reload skills.
