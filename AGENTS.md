# AGENTS.md

This file provides context for AI coding agents (GitHub Copilot, etc.) working in this repository.

## Project Overview

**notes-boost** is a personal learning notebook for [rwxrob's Beginner Boost](https://twitch.tv/rwxrob) — a live-streamed coding curriculum on Twitch. The repo contains:

- Sample code written during or after live sessions
- Searchable notes and references
- Exercises and experiments

The goal is a growing, well-organized reference that captures the journey from beginner to practitioner.

## Repository Structure

```
/
├── AGENTS.md           # AI agent context and preferences
├── PLAN.md             # Job-focused learning roadmap
└── README.md           # Project overview
```

## Development Environment

- **Container base**: `mcr.microsoft.com/devcontainers/base:ubuntu-24.04`
- **Tool manager**: [mise](https://mise.jdx.dev/) — config in `mise.toml`
- **Workspace manager**: DevPod — config in `.devcontainer/`
- **Setup**: run `.devcontainer/scripts/setup` (runs `mise trust` + `mise install`)
- **Clipboard**: `xclip` and `wl-clipboard` available

### Installed tools (mise.toml)

| Tool | Version |
|------|---------|
| gh   | latest  |

## Preferences

- Keep responses concise and direct
- Use [Conventional Commits](https://www.conventionalcommits.org/) for all commit messages (e.g. `feat:`, `fix:`, `docs:`, `chore:`)
- Never refer to any agent in any issue, PR, or commit message
- Always use `/usr/bin/open` (not `open`) when opening files or URLs on macOS

## Conventions

- No language/tooling conventions set yet — project is in early learning phase
- Notes will live in `notes/`, sample code in `code/` (not yet created)

## Notes for Agents

- Always read the **Progress** section below before responding
- Update the **Progress** section at the end of each session
- Refer to PLAN.md for the full learning roadmap

## Useful Commands

```sh
mise install          # Install/update all tools listed in mise.toml
gh repo view          # Open the GitHub repo summary
```

## Progress

- **Last session:** Not yet started
- **Topics covered:** Not yet
- **Up next:** Start Stage 1 of PLAN.md — terminal navigation and git basics; consider adding `notes/` and `code/` folder structure
