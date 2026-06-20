# kb-AutoBio — LLM Wiki Obsidian Vault

## Project Overview

Korean Obsidian vault for **AutoBio** research literature. Article notes are under `ko/articles/`.

## Repository Structure

```
.
├── ko/articles/   # Korean article notes
├── ko/pdf/        # PDF files (gitignored)
├── tools/         # Git submodule (git@github.com:taejoonlab/kb-tools.git)
└── .obsidian/     # Obsidian config (tracked, except workspace.json)
```

## Note Format

Every article note follows these sections in order:
1. `# Title` — full article title
2. `## Citation (NLM)` — NLM-formatted citation + DOI link
3. `## Background` — research background
4. `## Key Experiment Methods` — numbered methods
5. `## Results` — key findings
6. `## Perspective` — significance & future directions

## Git Conventions

- Clone with submodules: `git clone --recurse-submodules git@github.com:taejoonlab/kb-AutoBio.git`
- If already cloned without submodules: `git submodule update --init --recursive`
- Submodule URL uses **SSH** (`git@github.com:taejoonlab/kb-tools.git`) — ensure SSH key is configured
- `.gitignore` ignores: `.obsidian/workspace.json`, `.obsidian/cache/`, `.obsidian/plugins/obsidian-git/obsidian_askpass.sh`, `ko/pdf/`
- `filemode = false` in git config (cross-platform safe)

## Obsidian Setup

1. Open the cloned folder as an Obsidian vault
2. Community plugin **obsidian-git** is pre-configured but has auto-save/push/pull **disabled** (interval 0)
3. `tools/` is excluded from Obsidian file explorer via `userIgnoreFilters` in `.obsidian/app.json`

## AI Agent Rules

1. Filename convention: `FirstAuthorYYYY_Journal.md` (e.g., `Wu2021_NatComm.md`)
2. When adding a new article, create `ko/articles/FirstAuthorYYYY_Journal.md`
3. Do not modify files under `tools/` — that is a separate submodule repository
4. Do not modify `.obsidian/workspace.json` (per-machine state, gitignored)
5. Keep section order consistent: Title → Citation → Background → Key Experiment Methods → Results → Perspective
6. Commit messages should follow the pattern: `{action}: {description}` (e.g., `add: Wu2021_NatComm`, `edit: Haseeb2021_PNAS`)
