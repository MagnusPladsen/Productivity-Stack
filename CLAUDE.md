# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Documentation-only repository containing a curated list of free productivity tools and programs. Each category is a folder, each tool is an individual markdown file.

## Repository Structure

```
/
├── README.md              # Hub: title, intro, full TOC linking to all tool files
├── CONTRIBUTING.md        # Contributing guidelines and item template
├── CLAUDE.md
├── terminals/             # Terminal emulators
├── terminal-tools/        # CLI utilities and shell tools
├── editors/               # Code editors and Neovim distributions
├── note-taking/           # Note-taking applications
├── development-tools/     # API clients, databases, containers, debuggers
├── design-tools/          # Design and prototyping tools
├── ai-tools/              # AI coding agents and interfaces
├── package-managers/      # Package management tools
├── productivity-tools/    # Window managers, text expanders, launchers
├── image-editing/         # Image editors
└── browsers/              # Web browsers
```

Each category folder contains:
- `README.md` — category index with comparison table (Tool, Platforms, Open Source, Description)
- `tool-name.md` — individual tool files following the item template

## Conventions

- **Folder names:** kebab-case (e.g. `terminal-tools/`)
- **File names:** kebab-case `.md` (e.g. `oh-my-zsh.md`)
- **No subcategories** — all tools go directly in their category folder
- **Install commands:** per-OS sections, only for supported platforms, sourced from official docs
- **Alternatives:** relative links to similar tools in the repo (e.g. `[Kitty](kitty.md)`)
- **Platform tags:** only list platforms the tool actually supports
- **Free tier transparency:** if a tool is not 100% free, clearly state the free tier limits (e.g. "Free tier: 500 requests/month") in the tool file description. Never list a tool as simply "free" if it has usage caps, feature gates, or paid tiers
- **GitHub stars:** if a tool has a public GitHub repo, include the star count (e.g. `⭐ 28k`) in: the tool's `.md` file (after the GitHub link), the category `README.md` comparison table, and the root `README.md` TOC entry

## Adding a New Tool

1. Create `category/tool-name.md` following the item template in `CONTRIBUTING.md`
2. Add row to `category/README.md` comparison table
3. Add entry to root `README.md` TOC under the right category
