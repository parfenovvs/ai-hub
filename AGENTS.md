# ai-hub

Personal collection of agent skills, installed with the [`skills`](https://github.com/vercel-labs/skills) CLI (`npx skills add parfenovvs/ai-hub`).

## Repository Structure

```
ai-hub/
├── README.md        # Overview and install instructions
├── AGENTS.md        # This file — project structure and guidance for AI agents
└── skills/          # One directory per skill
    ├── commit/SKILL.md
    ├── jj/SKILL.md
    ├── new-feature/SKILL.md
    ├── pr/SKILL.md
    ├── tbd/SKILL.md
    └── vcs-workflow/SKILL.md
```

The `skills` CLI discovers every `skills/<name>/SKILL.md`. There is no manifest or catalog file.

## Skills

Each skill lives in `skills/<name>/SKILL.md` and contains:

- A YAML front-matter block with `name`, `description`, and trigger phrases
- Detailed instructions Claude follows when the skill is invoked

| Skill | Category | Description |
|-------|----------|-------------|
| [commit](skills/commit/SKILL.md) | vcs | Create conventional commit messages (feat, fix, docs, etc.) following the Conventional Commits spec |
| [jj](skills/jj/SKILL.md) | vcs | All version control operations using the Jujutsu (`jj`) CLI — commits, bookmarks, rebasing, workspaces |
| [new-feature](skills/new-feature/SKILL.md) | planning | Scaffold a new feature: gather requirements, create an isolated workspace, and produce a development plan before writing code |
| [pr](skills/pr/SKILL.md) | vcs | Create a pull request for the current branch with a structured description, using a repo template if one exists |
| [tbd](skills/tbd/SKILL.md) | planning | Plan and implement features as a stack of short-lived, independently-green PRs using trunk-based development |
| [vcs-workflow](skills/vcs-workflow/SKILL.md) | vcs | Unified VCS workflow: jj for local operations, gh for GitHub, trunk-based development with stacked PRs, and error recovery |

## Adding a New Skill

1. Create `skills/<name>/SKILL.md` with a YAML front-matter block (`name`, `description`) and skill body.
2. Add a row to the tables in `README.md` and `AGENTS.md`.
