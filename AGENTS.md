# AGENTS.md

This file provides context for AI coding agents (GitHub Copilot, etc.) working in this repository.

## Project Overview

**notes-boost** is a personal learning notebook for [rwxrob's Beginner Boost](https://twitch.tv/rwxrob) — a live-streamed coding curriculum on Twitch. The repo contains:

- Sample code written during or after live sessions
- Searchable notes and references
- Exercises and experiments

The goal is a growing, well-organized reference that captures the journey from beginner to practitioner.

## Repository Structure

> Update this section as the structure evolves.

```
/
├── AGENTS.md           # This file
├── mise.toml           # Tool versions managed by mise
└── .devcontainer/      # Dev container configuration
```

## Development Environment

- **Container base**: `mcr.microsoft.com/devcontainers/base:ubuntu-24.04`
- **Tool manager**: [mise](https://mise.jdx.dev/) — see `mise.toml` for pinned tool versions
- **Workspace manager**: DevPod
- **Setup**: run `.devcontainer/scripts/setup` (runs `mise trust` + `mise install`)
- **Clipboard**: `xclip` and `wl-clipboard` available

### Installed tools (mise.toml)

| Tool | Version |
|------|---------|
| gh   | latest  |

## Conventions & Preferences

- Keep notes in plain text or Markdown for easy searching (`grep`, `ripgrep`)
- Organize sample code into subdirectories named after the topic or session
- Prefer readable, commented code — this is a learning repo, not production

### AI assistant preferences

- Keep responses concise and direct
- Commit messages: imperative mood, lowercase subject line (e.g. `add notes on loops`)
- Never mention or reference any AI agent in issues, PRs, or commit messages

## Useful Commands

```sh
mise install          # Install/update all tools listed in mise.toml
gh repo view          # Open the GitHub repo summary
```
