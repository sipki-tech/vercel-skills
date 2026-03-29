# vercel-skill-cli-expert

Agent skill that provides complete expertise on the `npx skills` CLI — the open agent skills ecosystem tool by Vercel.

## Install

```bash
npx skills add Sipki-Tech/vercel-skills
```

Or install to specific agents:

```bash
npx skills add Sipki-Tech/vercel-skills -a claude-code -a cursor -a github-copilot
```

## What It Does

Once installed, your AI agent gains full knowledge of the `npx skills` CLI and can help you with:

- **Installing skills** — from GitHub, GitLab, local paths, with all flags and options
- **Removing skills** — by name, by agent, interactively, or all at once
- **Updating skills** — checking for updates and applying them
- **Listing & searching** — installed skills, filtering by agent, JSON output
- **Creating skills** — `SKILL.md` format, frontmatter, directory structure, publishing
- **Troubleshooting** — "No skills found", symlink issues, permission errors, CI/CD
- **Agent management** — 44+ supported agents, project vs global scope, paths

## Skill Structure

```
skills/vercel-skill-cli-expert/
├── SKILL.md                        # Decision flow & core procedures
├── references/
│   ├── commands.md                 # All 9 CLI commands with options & examples
│   ├── agents.md                   # 44+ agents: IDs, paths, compatibility
│   ├── skill-authoring.md          # Creating, structuring, publishing skills
│   └── troubleshooting.md          # Common errors, env vars, CI/CD patterns
└── assets/
    └── skill-template.md           # Ready-to-use SKILL.md template
```

## Covered Commands

| Command | Description |
|---|---|
| `skills add <package>` | Install skills from GitHub/GitLab/local path |
| `skills remove [skills]` | Remove installed skills |
| `skills list` | List installed skills |
| `skills find [query]` | Search for skills interactively |
| `skills check` | Check for available updates |
| `skills update` | Update all skills to latest |
| `skills init [name]` | Create a new SKILL.md template |
| `skills experimental_install` | Restore from skills-lock.json |
| `skills experimental_sync` | Sync skills from node_modules |

## Example Prompts

After installing, try asking your agent:

- "Install react best practices skills for Cursor and Claude Code"
- "How do I create my own skill and publish it?"
- "Remove all skills from Windsurf"
- "Set up CI/CD to auto-install skills"
- "What agents are supported and where do skills get installed?"
- "Why isn't my skill being discovered?"

## Requirements

- Node.js (for `npx`)
- `skills` CLI (runs via `npx skills`, no global install needed)

## License

MIT
