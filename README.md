# Temporal PHP Developer Skill

A coding-agent skill for building Temporal applications with the **PHP SDK**.
Forked from [temporalio/skill-temporal-developer](https://github.com/temporalio/skill-temporal-developer) (PR [#40](https://github.com/temporalio/skill-temporal-developer/pull/40)), trimmed to PHP only.

## Installation

### Any agent (via `npx skills`)

```bash
npx skills add algirdasci/skill-temporal-developer
```

Follow the prompts to pick your agent and scope.

### Manual (agent-agnostic)

Clone into your agent's skills directory:

```bash
# Claude Code
git clone https://github.com/algirdasci/skill-temporal-developer ~/.claude/skills/temporal-php-developer

# pi
git clone https://github.com/algirdasci/skill-temporal-developer ~/.pi/agent/skills/temporal-php-developer

# Project-scoped (any agent that reads .agent/skills or similar)
git clone https://github.com/algirdasci/skill-temporal-developer .agent/skills/temporal-php-developer
```

Adjust the directory to your agent's convention — the repo is a standard skill: `SKILL.md` at the root plus `references/`.

## What's inside

- `SKILL.md` — entry point: architecture, determinism, CLI setup
- `references/core/` — language-agnostic concepts (patterns, gotchas, versioning, troubleshooting, errors)
- `references/php/` — PHP SDK guides (setup, testing, patterns, observability, error handling, data handling, versioning)

## Syncing with upstream

```bash
git remote add upstream https://github.com/temporalio/skill-temporal-developer.git
git fetch upstream
git merge upstream/feature/add-php-support   # or upstream/main once PR #40 is merged
```
