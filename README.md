# pvs-claude-marketplace — Agent Skills

A personal collection of reusable agent skills, installable with the [`skills`](https://github.com/vercel-labs/skills) CLI.

## Install

List available skills:

```
npx skills add parfenovvs/pvs-claude-marketplace -l
```

Install all skills:

```
npx skills add parfenovvs/pvs-claude-marketplace
```

Install a single skill:

```
npx skills add parfenovvs/pvs-claude-marketplace --skill commit
```

## Skills

| Skill | Category | Description |
|-------|----------|-------------|
| [commit](skills/commit/SKILL.md) | vcs | Create conventional commit messages (feat, fix, docs, etc.) following the Conventional Commits spec |
| [jj](skills/jj/SKILL.md) | vcs | All version control operations using the Jujutsu (`jj`) CLI — commits, bookmarks, rebasing, workspaces |
| [pr](skills/pr/SKILL.md) | vcs | Create a pull request for the current branch with a structured description, using a repo template if one exists |
| [new-feature](skills/new-feature/SKILL.md) | planning | Scaffold a new feature: gather requirements, create an isolated workspace, and produce a development plan before writing code |
| [tbd](skills/tbd/SKILL.md) | planning | Plan and implement features as a stack of short-lived, independently-green PRs using trunk-based development |
| [vcs-workflow](skills/vcs-workflow/SKILL.md) | vcs | Unified VCS workflow: jj for local operations, gh for GitHub, trunk-based development with stacked PRs, and error recovery |
