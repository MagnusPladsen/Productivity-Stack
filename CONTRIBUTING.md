# Contributing

Want to add your favorite tools to this list? Follow these steps:

1. Fork this repository.
2. Create a new `.md` file in the appropriate category folder using the item template below.
3. Add the tool to the category's `README.md` comparison table.
4. Add the tool to the root `README.md` Table of Contents.
5. Submit a pull request.

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

## Conventions

- **Folder names:** kebab-case (e.g. `terminal-tools/`)
- **File names:** kebab-case `.md` (e.g. `oh-my-zsh.md`)
- **Category index:** Each folder has a `README.md` with a comparison table
- **Install commands:** Only include platforms the tool supports. Source commands from official docs.
- **No subcategories:** All tools go directly in their category folder
