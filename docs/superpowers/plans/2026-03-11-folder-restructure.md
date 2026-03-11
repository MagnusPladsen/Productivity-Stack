# Folder Restructure Implementation Plan

> **For agentic workers:** REQUIRED: Use superpowers:subagent-driven-development (if subagents available) or superpowers:executing-plans to implement this plan. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Restructure the Productivity Stack repo from a single README.md into a folder-based layout with category folders, tool markdown files, per-OS install commands, and comparison tables.

**Architecture:** Each category becomes a kebab-case folder with a `README.md` index (comparison table) and individual `tool-name.md` files. Root README.md becomes a hub linking to all items. Each tool file contains description, platform tags, links, per-OS install commands, and alternatives.

**Tech Stack:** Markdown, GitHub-flavored markdown tables, web search for install commands

**Spec:** `docs/superpowers/specs/2026-03-11-folder-restructure-design.md`

---

## Chunk 1: Scaffolding and Meta Files

### Task 1: Create all category folders

**Files:**
- Create: `terminals/`, `terminal-tools/`, `editors/`, `note-taking/`, `development-tools/`, `design-tools/`, `ai-tools/`, `package-managers/`, `productivity-tools/`, `image-editing/`, `browsers/`

- [ ] **Step 1: Create all 11 category directories**

```bash
mkdir -p terminals terminal-tools editors note-taking development-tools design-tools ai-tools package-managers productivity-tools image-editing browsers
```

- [ ] **Step 2: Verify directories exist**

```bash
ls -d */
```

Expected: All 11 directories listed.

- [ ] **Step 3: Commit**

```bash
git add .
git commit -m "scaffold: create category folders"
```

---

### Task 2: Create CONTRIBUTING.md

**Files:**
- Create: `CONTRIBUTING.md`

- [ ] **Step 1: Create CONTRIBUTING.md**

```markdown
# Contributing

Want to add your favorite tools to this list? Follow these steps:

1. Fork this repository.
2. Create a new `.md` file in the appropriate category folder using the item template below.
3. Add the tool to the category's `README.md` comparison table.
4. Add the tool to the root `README.md` Table of Contents.
5. Submit a pull request.

## Item File Template

\`\`\`markdown
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
\`\`\`

## Conventions

- **Folder names:** kebab-case (e.g. `terminal-tools/`)
- **File names:** kebab-case `.md` (e.g. `oh-my-zsh.md`)
- **Category index:** Each folder has a `README.md` with a comparison table
- **Install commands:** Only include platforms the tool supports. Source commands from official docs.
- **No subcategories:** All tools go directly in their category folder
```

- [ ] **Step 2: Commit**

```bash
git add CONTRIBUTING.md
git commit -m "docs: add CONTRIBUTING.md with conventions and template"
```

---

### Task 3: Update CLAUDE.md with folder conventions

**Files:**
- Modify: `CLAUDE.md`

- [ ] **Step 1: Add structure and conventions section to CLAUDE.md**

Add after the existing content:

```markdown
## Repository Structure

Each category is a kebab-case folder with:
- `README.md` — category index with comparison table (Tool, Platforms, Open Source, Description)
- `tool-name.md` — individual tool files following the item template

### Conventions
- Folder names: kebab-case (e.g. `terminal-tools/`)
- File names: kebab-case `.md` (e.g. `oh-my-zsh.md`)
- No subcategories — all tools go directly in their category folder
- Install commands: per-OS sections, only for supported platforms, sourced from official docs
- Alternatives: relative links to similar tools in the repo
- Platform tags: only list platforms the tool actually supports

### Categories
terminals, terminal-tools, editors, note-taking, development-tools, design-tools, ai-tools, package-managers, productivity-tools, image-editing, browsers

### Adding a new tool
1. Create `category/tool-name.md` following the item template in CONTRIBUTING.md
2. Add row to `category/README.md` comparison table
3. Add entry to root `README.md` TOC under the right category
```

- [ ] **Step 2: Commit**

```bash
git add CLAUDE.md
git commit -m "docs: add folder structure conventions to CLAUDE.md"
```

---

## Chunk 2: Terminals (5 items)

### Task 4: Create terminal tool files

**Files:**
- Create: `terminals/kitty.md`, `terminals/iterm2.md`, `terminals/warp.md`, `terminals/ghostty.md`, `terminals/cmux.md`

For each tool file:
- [ ] **Step 1: Web search** the tool's official site and/or GitHub repo for: platforms supported, install commands per OS (brew, apt, winget, scoop, etc.), GitHub repo URL
- [ ] **Step 2: Create the .md file** following the item template with description, platform tags, links, per-OS install commands, and alternatives (link to other terminals)
- [ ] **Step 3: Repeat** for all 5 terminals

Tools and known links:
- **Kitty**: https://sw.kovidgoyal.net/kitty/ — macOS, Linux
- **iTerm2**: https://iterm2.com/ — macOS only
- **Warp**: https://www.warp.dev/ — macOS, Linux, Windows
- **Ghostty**: https://github.com/ghostty-org/ghostty — macOS, Linux
- **cmux**: https://www.cmux.dev/ — macOS only

- [ ] **Step 4: Create `terminals/README.md`** with category description and comparison table

```markdown
# Terminals

Terminal emulators for your development workflow.

| Tool | Platforms | Open Source | Description |
|------|-----------|-------------|-------------|
| [Kitty](kitty.md) | macOS, Linux | Yes | GPU-accelerated terminal emulator |
| [iTerm2](iterm2.md) | macOS | Yes | Feature-rich terminal with split panes and search |
| [Warp](warp.md) | macOS, Linux, Windows | No | AI-powered terminal with command prediction |
| [Ghostty](ghostty.md) | macOS, Linux | Yes | Modern terminal focused on performance |
| [cmux](cmux.md) | macOS | Yes | Ghostty-based terminal for AI coding agents |
```

- [ ] **Step 5: Commit**

```bash
git add terminals/
git commit -m "feat: add terminals category with 5 tool files"
```

---

## Chunk 3: Terminal Tools (24 items)

### Task 5: Create terminal tool files (batch 1: oh-my-zsh through fzf — 10 items)

**Files:**
- Create: `terminal-tools/oh-my-zsh.md`, `terminal-tools/lazygit.md`, `terminal-tools/tmux.md`, `terminal-tools/zoxide.md`, `terminal-tools/bat.md`, `terminal-tools/eza.md`, `terminal-tools/ripgrep.md`, `terminal-tools/fd.md`, `terminal-tools/htop.md`, `terminal-tools/fzf.md`

For each tool:
- [ ] **Step 1: Web search** for platforms, install commands, GitHub URL
- [ ] **Step 2: Create .md file** with template content
- [ ] **Step 3: Repeat** for all 10 tools

- [ ] **Step 4: Commit**

```bash
git add terminal-tools/
git commit -m "feat: add terminal tools batch 1 (oh-my-zsh through fzf)"
```

---

### Task 6: Create terminal tool files (batch 2: git through jolt — 14 items)

**Files:**
- Create: `terminal-tools/git.md`, `terminal-tools/curl.md`, `terminal-tools/tldr.md`, `terminal-tools/jq.md`, `terminal-tools/ncdu.md`, `terminal-tools/asciinema.md`, `terminal-tools/taproom.md`, `terminal-tools/fastfetch.md`, `terminal-tools/figlet.md`, `terminal-tools/thefuck.md`, `terminal-tools/gh.md`, `terminal-tools/yazi.md`, `terminal-tools/jolt.md`

For each tool:
- [ ] **Step 1: Web search** for platforms, install commands, GitHub URL
- [ ] **Step 2: Create .md file** with template content
- [ ] **Step 3: Repeat** for all 13 tools

Note: **Jolt** is a new addition — https://github.com/jordond/jolt — battery/energy monitor TUI.

- [ ] **Step 4: Commit**

```bash
git add terminal-tools/
git commit -m "feat: add terminal tools batch 2 (git through jolt)"
```

---

### Task 7: Create terminal-tools/README.md

**Files:**
- Create: `terminal-tools/README.md`

- [ ] **Step 1: Create comparison table** with all 24 tools (oh-my-zsh, lazygit, tmux, zoxide, bat, eza, ripgrep, fd, htop, fzf, git, curl, tldr, jq, ncdu, asciinema, taproom, fastfetch, figlet, thefuck, gh, yazi, jolt)

- [ ] **Step 2: Commit**

```bash
git add terminal-tools/README.md
git commit -m "feat: add terminal-tools category index"
```

---

## Chunk 4: Editors (8 items, includes former Neovim Distributions)

### Task 8: Create editor tool files

**Files:**
- Create: `editors/zed.md`, `editors/neovim.md`, `editors/neovide.md`, `editors/vscode.md`, `editors/astronvim.md`, `editors/lazyvim.md`, `editors/nvchad.md`

For each tool:
- [ ] **Step 1: Web search** for platforms, install commands, GitHub URL
- [ ] **Step 2: Create .md file** with template content
- [ ] **Step 3: Repeat** for all 7 editors

For AstroNvim, LazyVim, NvChad — these are Neovim distributions/configs. Install is typically cloning a repo, not brew. Document accordingly. Alternatives should cross-link each other.

- [ ] **Step 4: Create `editors/README.md`** with comparison table

- [ ] **Step 5: Commit**

```bash
git add editors/
git commit -m "feat: add editors category with 7 tool files (includes neovim distros)"
```

---

## Chunk 5: Remaining Categories (6 categories, 28 items)

### Task 9: Note Taking (3 items)

**Files:**
- Create: `note-taking/obsidian.md`, `note-taking/joplin.md`, `note-taking/notion.md`, `note-taking/README.md`

- [ ] **Step 1:** Web search + create all 3 tool files
- [ ] **Step 2:** Create README.md with comparison table
- [ ] **Step 3: Commit**

```bash
git add note-taking/
git commit -m "feat: add note-taking category with 3 tool files"
```

---

### Task 10: Development Tools (8 items)

**Files:**
- Create: `development-tools/bruno.md`, `development-tools/dbeaver.md`, `development-tools/docker.md`, `development-tools/insomnia.md`, `development-tools/postman.md`, `development-tools/shadcn-cli.md`, `development-tools/rad-debugger.md`, `development-tools/renderdoc.md`, `development-tools/README.md`

- [ ] **Step 1:** Web search + create all 8 tool files
- [ ] **Step 2:** Create README.md with comparison table
- [ ] **Step 3: Commit**

```bash
git add development-tools/
git commit -m "feat: add development-tools category with 8 tool files"
```

---

### Task 11: Design Tools (3 items)

**Files:**
- Create: `design-tools/penpot.md`, `design-tools/modulz.md`, `design-tools/draw-io.md`, `design-tools/README.md`

- [ ] **Step 1:** Web search + create all 3 tool files
- [ ] **Step 2:** Create README.md with comparison table
- [ ] **Step 3: Commit**

```bash
git add design-tools/
git commit -m "feat: add design-tools category with 3 tool files"
```

---

### Task 12: AI Tools (7 items)

**Files:**
- Create: `ai-tools/open-webui.md`, `ai-tools/open-router.md`, `ai-tools/claude-code-terminal.md`, `ai-tools/crush.md`, `ai-tools/codex-app.md`, `ai-tools/codex-cli-terminal.md`, `ai-tools/opencode.md`, `ai-tools/README.md`

- [ ] **Step 1:** Web search + create all 7 tool files
- [ ] **Step 2:** Create README.md with comparison table
- [ ] **Step 3: Commit**

```bash
git add ai-tools/
git commit -m "feat: add ai-tools category with 7 tool files"
```

---

### Task 13: Package Managers, Productivity Tools, Image Editing, Browsers (12 items)

**Files:**
- Create: `package-managers/homebrew.md`, `package-managers/README.md`
- Create: `productivity-tools/espanso.md`, `productivity-tools/raycast.md`, `productivity-tools/alttab.md`, `productivity-tools/rectangle.md`, `productivity-tools/aerospace.md`, `productivity-tools/sketchybar.md`, `productivity-tools/janky-borders.md`, `productivity-tools/cheatsheet.md`, `productivity-tools/README.md`
- Create: `image-editing/gimp.md`, `image-editing/krita.md`, `image-editing/README.md`
- Create: `browsers/zen-browser.md`, `browsers/README.md`

- [ ] **Step 1:** Web search + create all tool files for package-managers (1)
- [ ] **Step 2:** Create package-managers/README.md
- [ ] **Step 3: Commit**

```bash
git add package-managers/
git commit -m "feat: add package-managers category"
```

- [ ] **Step 4:** Web search + create all tool files for productivity-tools (8)
- [ ] **Step 5:** Create productivity-tools/README.md
- [ ] **Step 6: Commit**

```bash
git add productivity-tools/
git commit -m "feat: add productivity-tools category with 8 tool files"
```

- [ ] **Step 7:** Web search + create all tool files for image-editing (2)
- [ ] **Step 8:** Create image-editing/README.md
- [ ] **Step 9: Commit**

```bash
git add image-editing/
git commit -m "feat: add image-editing category with 2 tool files"
```

- [ ] **Step 10:** Web search + create zen-browser.md
- [ ] **Step 11:** Create browsers/README.md
- [ ] **Step 12: Commit**

```bash
git add browsers/
git commit -m "feat: add browsers category"
```

---

## Chunk 6: Root README.md and Cleanup

### Task 14: Rewrite root README.md

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Rewrite README.md** as hub with:
  - Title + intro
  - Full TOC organized by category
  - Category headings link to `category/README.md`
  - Every item links to its `category/tool-name.md` file

Format per category:
```markdown
### [Terminals](terminals/README.md)
- [Kitty](terminals/kitty.md)
- [iTerm2](terminals/iterm2.md)
...
```

- [ ] **Step 2: Verify all links** are correct relative paths

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: rewrite root README as hub linking to all tool files"
```

---

### Task 15: Final verification and cleanup

- [ ] **Step 1: Count files** — verify we have the expected number of .md files across all folders

```bash
find . -name "*.md" -not -path "./.git/*" -not -path "./docs/*" | wc -l
```

Expected: ~75 files (11 category READMEs + ~60 tool files + root README + CONTRIBUTING + CLAUDE.md)

- [ ] **Step 2: Check for broken links** — spot-check that category README tables link to existing files

- [ ] **Step 3: Final commit if any fixes needed**

```bash
git add -A
git commit -m "fix: address any broken links or missing files"
```

- [ ] **Step 4: Push**

```bash
git push
```

---

## Parallelization Guide

Tasks that can run in parallel (independent categories):
- **Tasks 4-7** (Terminals + Terminal Tools) can run in parallel with **Task 8** (Editors)
- **Tasks 9-13** (all remaining categories) can all run in parallel with each other
- **Task 14** (root README) depends on ALL category tasks being complete
- **Task 15** (verification) depends on Task 14
