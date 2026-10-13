# T-NEWPROJECT-T

This is a template repository cloned into every new project.

Project-specific rules, formatting guidelines, and skill definitions live in `.agents/`.

See `.agents/rules/` for agent communication style, date/time formats, typography conventions (no em/en dashes, no smart quotes, no bold-as-emphasis), writing style, and git file-move rules (`git mv` for tracked files).

See `.agents/skills/` for mode-specific instructions: `bun-instead-of-node` (use Bun for all runtime operations), `caveman` (ultra-compressed response mode), `dt-technical-writer` (Distilled Technical writing), `lint-md` (markdownlint workflow), and `obsidian-markdown` (Obsidian Flavored Markdown syntax).

Markdown linting: `.markdownlint-cli2.jsonc` configures markdownlint-cli2. Run `bun x markdownlint-cli2 --fix "**/*.md"` from the project root. The linter runs automatically on save via VS Code settings (`.vscode/settings.json`). See `.agents/skills/lint-md/SKILL.md` for the full workflow.

VS Code: recommended extensions in `.vscode/extensions.json` (vscode-markdownlint, Notepad++ keybindings). Settings enable on-type markdownlint auto-fix.

Obsidian: plugin data and configuration live in `.obsidian/`. See `.agents/skills/obsidian-markdown/SKILL.md` for wikilink, embed, callout, and property syntax.
