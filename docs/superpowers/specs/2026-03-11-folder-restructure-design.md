# Folder Restructure Design

## Summary

Restructure the Productivity Stack repository from a single README.md into a folder-based layout where each category is a folder with an index README.md, and each tool is an individual markdown file with detailed info, install commands per OS, links, platform tags, and alternatives.

## Folder Structure

```
/
├── README.md                    # Hub: title, intro, full TOC linking to all item files
├── CONTRIBUTING.md              # Contributing guidelines (extracted from README)
├── CLAUDE.md
├── terminals/
│   ├── README.md                # Category index with comparison table
│   ├── kitty.md
│   ├── iterm2.md
│   ├── warp.md
│   ├── ghostty.md
│   └── cmux.md
├── terminal-tools/
│   ├── README.md
│   ├── oh-my-zsh.md
│   ├── lazygit.md
│   ├── tmux.md
│   ├── zoxide.md
│   ├── bat.md
│   ├── eza.md
│   ├── ripgrep.md
│   ├── fd.md
│   ├── htop.md
│   ├── fzf.md
│   ├── git.md
│   ├── curl.md
│   ├── tldr.md
│   ├── jq.md
│   ├── ncdu.md
│   ├── asciinema.md
│   ├── taproom.md
│   ├── fastfetch.md
│   ├── figlet.md
│   ├── thefuck.md
│   ├── gh.md
│   ├── yazi.md
│   └── jolt.md
├── editors/
│   ├── README.md
│   ├── zed.md
│   ├── neovim.md
│   ├── neovide.md
│   ├── vscode.md
│   ├── astronvim.md
│   ├── lazyvim.md
│   └── nvchad.md
├── note-taking/
│   ├── README.md
│   ├── obsidian.md
│   ├── joplin.md
│   └── notion.md
├── development-tools/
│   ├── README.md
│   ├── bruno.md
│   ├── dbeaver.md
│   ├── docker.md
│   ├── insomnia.md
│   ├── postman.md
│   ├── shadcn-cli.md
│   ├── rad-debugger.md
│   └── renderdoc.md
├── design-tools/
│   ├── README.md
│   ├── penpot.md
│   ├── modulz.md
│   └── draw-io.md
├── ai-tools/
│   ├── README.md
│   ├── open-webui.md
│   ├── open-router.md
│   ├── claude-code-terminal.md
│   ├── crush.md
│   ├── codex-app.md
│   ├── codex-cli-terminal.md
│   └── opencode.md
├── package-managers/
│   ├── README.md
│   └── homebrew.md
├── productivity-tools/
│   ├── README.md
│   ├── espanso.md
│   ├── raycast.md
│   ├── alttab.md
│   ├── rectangle.md
│   ├── aerospace.md
│   ├── sketchybar.md
│   ├── janky-borders.md
│   └── cheatsheet.md
├── image-editing/
│   ├── README.md
│   ├── gimp.md
│   └── krita.md
└── browsers/
    ├── README.md
    └── zen-browser.md
```

## Item File Template

```markdown
# Tool Name

> One-line description.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://...)
- [GitHub Repository](https://github.com/...)

## Install

### macOS
\`\`\`bash
brew install tool-name
\`\`\`

### Linux
\`\`\`bash
sudo apt install tool-name
\`\`\`

### Windows
\`\`\`bash
winget install tool-name
\`\`\`

## Alternatives
- [Similar Tool](../category/similar-tool.md)
```

### Item file rules

- Only include install sections for platforms the tool actually supports
- Install commands sourced from official site/repo — no guessing
- If a platform only has a manual download, link to the download page
- Alternatives use relative links to other items in the repo
- Platform tags reflect actual support

## Category Index (README.md) Template

```markdown
# Category Name

Short description of what this category covers.

| Tool | Platforms | Open Source | Description |
|------|-----------|-------------|-------------|
| [Tool](tool.md) | macOS, Linux | Yes | One-line description |
```

## Root README.md

- Title + intro paragraph
- Full Table of Contents organized by category
- Category headings link to the category README.md (e.g. `[Terminals](terminals/README.md)`)
- Every individual item links to its `.md` file (e.g. `[Kitty](terminals/kitty.md)`)

## CONTRIBUTING.md

Extracted from current README. Contains fork/add/PR instructions, plus the new conventions:
- Tools go in the appropriate category folder as a `.md` file
- Follow the item file template
- Add the tool to the category's README.md comparison table
- Add the tool to the root README.md TOC

## CLAUDE.md Rules

Add rules documenting:
- Folder naming: kebab-case
- File naming: kebab-case `.md`
- Category index: `README.md` per folder
- Item file template structure
- No subcategories

## New Items

- **Jolt** — terminal-based battery and energy monitor → `terminal-tools/jolt.md`

## Decisions

- Folder names: kebab-case
- File names: kebab-case `.md`
- Category indexes: `README.md` (GitHub auto-renders)
- Neovim Distributions: merged into `editors/` (no subcategories)
- Contributing: extracted to `CONTRIBUTING.md`
- Install commands: per-OS sections, only for supported platforms
- Platforms: tagged per tool
- Alternatives: relative links to similar tools in the repo
